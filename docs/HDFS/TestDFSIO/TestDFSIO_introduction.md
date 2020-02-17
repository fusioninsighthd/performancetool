# TestDFSIO工具介绍

## 1. 简介

TestDFSIO 工具为Hadoop源码中自带的一种测试工具，可以通过源码构建获得，工具名称一般为

`hadoop-mapreduce-client-jobclient-[版本号]-test.jar`。

开源hadoop源码地址：https://github.com/apache/hadoop

开源编译构建过程可参考：https://www.cnblogs.com/bclshuai/p/12009991.html

TestDFSIO作为一种分布式I/O Benchmark测试工具。

## 2. 使用指导

该工具通过命令行形式使用，使用参考：

```shell
#yarn jar /opt/client/HDFS/hadoop/share/hadoop/mapreduce/hadoop-mapreduce-client-jobclient-3.1.1-tests.jar  TestDFSIO

Usage: TestDFSIO [genericOptions] -read [-random | -backward | -skip [-skipSize Size]] | -write | -append | -truncate | -clean [-compression codecClassName] [-nrFiles N] [-size Size[B|KB|MB|GB|TB]] [-resFile resultFileName] [-bufferSize Bytes] [-storagePolicy storagePolicyName] [-erasureCodePolicy erasureCodePolicyName]

```

genericOptions  通用选项，参考 如下

![](..\assets\hadoop_command_generic_options.png)

- -read 读测试
- -write 写测试
- -append 追加测试，每个文件追加-size指定的数据量
- -truncate 截断测试，每个文件截断至-size指定的数据量
- -clean：清除TestDFSIO在HDFS上生成数据
- -n：文件个数
- -size：每个文件的大小
- -resFile：生成测试报告的本地文件路径
- -bufferSize：每个mapper任务读写文件所用到的缓存区大小，默认为1000000字节。

## 3. 参考

http://blog.sina.com.cn/s/blog_72ef7bea0102vr44.html

https://hadoop.apache.org/docs/r3.1.1/hadoop-project-dist/hadoop-common/CommandsManual.html#Generic_Options



