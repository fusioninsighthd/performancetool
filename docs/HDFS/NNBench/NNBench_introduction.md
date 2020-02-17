# NNBench工具介绍

## 1. 简介

NNBench 工具为Hadoop源码中自带的一种测试工具，可以通过源码构建获得，工具名称一般为

`hadoop-mapreduce-client-jobclient-[版本号]-test.jar`。

开源hadoop源码地址：https://github.com/apache/hadoop

开源编译构建过程可参考：https://www.cnblogs.com/bclshuai/p/12009991.html

NNBench工具用于测试HDFS的Namenode的能力。

## 2. 使用指导

### 2.1 命令行参数

该工具通过命令行形式使用，使用参考：

```shell
# hadoop jar /opt/client/HDFS/hadoop/share/hadoop/mapreduce/hadoop-mapreduce-client-jobclient-3.1.1-tests.jar nnbench
NameNode Benchmark 0.4
Usage: nnbench <options>
Options:
-operation <Available operations are create_write open_read rename delete. This option is mandatory>
 * NOTE: The open_read, rename and delete operations assume that the files they operate on, are already available. The create_write operation must be run before running the other operations.
-maps <number of maps. default is 1. This is not mandatory>
-reduces <number of reduces. default is 1. This is not mandatory>
-startTime <time to start, given in seconds from the epoch. Make sure this is far enough into the future, so all maps (operations) will start at the same time. default is launch time + 2 mins. This is not mandatory>
-blockSize <Block size in bytes. default is 1. This is not mandatory>
-bytesToWrite <Bytes to write. default is 0. This is not mandatory>
-bytesPerChecksum <Bytes per checksum for the files. default is 1. This is not mandatory>
-numberOfFiles <number of files to create. default is 1. This is not mandatory>
-replicationFactorPerFile <Replication factor for the files. default is 1. This is not mandatory>
-baseDir <base DFS path. default is /benchmarks/NNBench. This is not mandatory>
-readFileAfterOpen <true or false. if true, it reads the file and reports the average time to read. This is valid with the open_read operation. default is false. This is not mandatory>
-help: Display the help statement
```

- -operation [必有参数]可选 create_write open_read rename delete

- -maps [可选参数]

- -reduces

- -blockSize

- -bytesToWrite

- -bytesPerChecksum

- -numberOfFiles

- -replicationFactorPerFile

- -baseDir

- -readFileAfterOpen

### 2.2 处理逻辑

1. 输入检查是否合法
2. cleanupBeforeTestrun 删除已有的基于-baseDir的数据
3. createControlFiles 生成控制文件基于baseDir/CONTROL_DIR_NAME/NNBench_Controlfile_i(numberOfMaps)
4. 执行mapper的时候基于controlfile生成mapper个数，每个mapper基于operation 进行相应的操作，如doCreateWriteOp每个mapper又基于numberOfFiles生成numberOfFiles个文件
5. 执行reducer时写入统计的信息
6. 对写入的统计信息做分析出result

## 3. 参考





