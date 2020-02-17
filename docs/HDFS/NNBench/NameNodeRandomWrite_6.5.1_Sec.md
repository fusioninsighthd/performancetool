# NameNode随机写性能测试

## 1. 支持版本

FusionInsight HD 6.5.1

## 2. 工具下载
因涉及源码编译，需调用实际源码，过程比较复杂，故该工具给出直接下载链接：<br/><a href="../hdfs-6.5.1.zip">【6.5.1工具下载链接】</a>
<br/>校验md5:<span class="label label-Pass ">9b301864b41909b67b80d8f59d74ef32</span>  hdfs-6.5.1.zip

## 3. 测试步骤
### 3.1 前置条件
- FI集群安装为安全模式，且运行正常
- HDFS、MapReduce、Yarn服务正常
- 已于linux环境安装集群客户端，客户端安装<a href="../../../fusioninsight_client">[步骤参考]</a>
- 已配置具有HDFS\Yarn访问权限的用户，例如用户名poc，并对poc用户有对应的Yarn资源分配

### 3.2 测试过程

1. 【可选】参考产品文档中”规划HDFS容量“部分，修改GC_OPTS的参数；

2. 修改HDFS如下配置项，重启服务

   ```
   dfs.namenode.handler.count : 512
   dfs.datanode.handler.count : 128
   ipc.server.handler.queue.size : 200
   dfs.namenode.fs-limits.max-directory-items : 6400000
   ```
3. 修改Yarn配置项，重启服务

   ```
   yarn.nodemanager.resource.cpu-vcores  根据实际节点的CPU核数修改
   yarn.nodemanager.resource.memory-mb   根据实际节点的内存修改
   ```
4. 修改租户资源池中配置的`Maximum AM Resource Percent`为`0.9`<br />
5. 将测试工具解压缩后上传到客户端，如果客户端安装在`/opt/client`目录下，那么工具上传的路径为`/opt/client/HDFS/hadoop/share/hadoop/mapreduce/`目录下<br />
6. 执行安全认证

   ```
   source /opt/client/bigdata_env
   kinit pc
   ```
7. 启动测试

```shell
yarn jar /opt/client/HDFS/hadoop/share/hadoop/mapreduce/hadoop-mapreduce-client-jobclient-3.1.1-tests.jar nnbench  \
-operation create_write \ 
-maps 10 \ 
-reduces 2 \
-bytesToWrite 1 \
-numberOfFiles 100 \
-blockSize 1048576 \
-replicationFactorPerFile 3 \
-readFileAfterOpen true \
-baseDir /benchmarks1/NNBench
```

参数说明：
```
-maps		 指定MR任务的map数，必须保证map数都在同一轮并发中，否则结果计算有误
-reduces		指定MR任务的reduce数，结果汇总，可写一个比较小的数字，不影响结果
-bytesToWrite	创建文件的实际大小
-numberOfFiles	每个map任务创建的文件数
-blockSize		文件块的大小，默认是128MB，这里取1048576字节为1MB
-replicationFactorPerFile	文件副本数
-readFileAfterOpen	是否读取文件
-baseDir	创建的HDFS上的路径
```
### 3.3 查看测试结果
测试完毕，参考当前目录下的`NNBench_results.log`内容获取Namenode处理性能数据

![](..\assets\nnbench1.png)