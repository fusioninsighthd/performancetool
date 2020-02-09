
<!-- ex_nonav -->

# FusionInsight HD测试工具汇总

华为FusionInsight HD支持开源标准的Hadoop接口，兼容开源的Hadoop测试工具，因部分开源工具未考虑安全认证，故给出开源工具适配华为FI HD集群的测试操作指导！
</br>使用maven构建的依赖包下载地址为<a href="https://support.huawei.com/enterprise/zh/cloud-computing/fusioninsight-tool-pid-21624171/software/250709838?idAbsPath=fixnode01%7C7919749%7C7941815%7C19942925%7C21624171
">[6.5.1maven源]</a>，下载后覆盖本地maven仓库即可！

<table class="tg">
 <thead>
 <tr>
  <td colspan=4 >测试工具</td>
  <td colspan=4>FusionInsight</td>
 </tr>
 <tr>
  <td rowspan=2>组件名称</td>
  <td rowspan=2>工具名称</td>
  <td rowspan=2 class="">开源源码</br>FI安全认证源码</td>
  <td rowspan=2>测试场景</td>
  <td rowspan=1 colspan=2>8.0</td>
  <td rowspan=1 colspan=2>6.5.1</td>
 </tr>
 <tr>
 <td>安全集群</td>
 <td>普通集群</td>
 <td>安全集群</td>
 <td>普通集群</td>
 </tr>
</thead>
<!-- 如下是HDFS部分 -->
<tr>
	<td rowspan=4 ><img class="navbar-logo" src="https://hadoop.apache.org/elephant.png"></i></br>HDFS</td>

	<td rowspan=4 >TestDFSIO</td>
	<td rowspan=4 >
		<a href="https://github.com/hortonworks/hive-testbench">[源码github]</a>
		</br>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
	</td>
	
		<td>NameNode随机写性能</td>
		<td>
		<!--<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a> -->
		<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a> 
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未 验证&nbsp;</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未  验 证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未  验 证</span></a>
		</td>
	
		<tr>
		<td>NameNode随机读性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>
		
		<tr>
		<td>DataNode随机写性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>
		
		<tr>
		<td>DataNode随机读性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>
</tr>

<!-- 如下是Yarn部分 -->
<tr>
	<td rowspan=4 ><img class="navbar-logo" src="https://hadoop.apache.org/elephant.png"><i aria-hidden="true"></i></br>Yarn</td>
	<td rowspan=4 >HiBench6.0</td>
	<td rowspan=4 >
		<a href="https://github.com/hortonworks/hive-testbench">[源码github]</a>
		</br>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
	</td>
		<td>TeraSort</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		
		<tr>
		<td>WordCount</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>

		<tr>
		<td>贝叶斯分类(Bayes)</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>

		<tr>
		<td>K均值聚类(Kmeans)</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>
</tr>


<!-- 如下是Hive部分 -->
<tr>
<td rowspan=1 ><img class="navbar-logo" src="https://hive.apache.org/images/hive_logo_medium.jpg"><i aria-hidden="true"></i></br>Hive</td>
		<td>TPC-DS</td>
		<td>
		<a href="https://github.com/hortonworks/hive-testbench">[源码github]</a>
		</br>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
		</td>
				<td>hive-testbench测试通用SQL</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
</tr>

<!-- 如下是HBase部分 -->
<tr>
<td rowspan=3 ><img class="navbar-logo" src="https://hbase.apache.org/images/hbase_logo_with_orca_large.png"><i aria-hidden="true"></i></br>HBase</td>
		<td>PerformanceEvaluation</td>
		<td>
		<a href="https://github.com/hortonworks/hive-testbench">[源码github]</a>
		</br>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
		</td>
		<td>HBase源码自带测试工具</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>

	<tr>
		<td>YCSB</td>
		<td>
		<a href="https://github.com/brianfrankcooper/YCSB">[源码github]</a>
		</br>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
		</td>
		<td>雅虎测试工具</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
	</tr>
	
	<tr>
		<td>bulkload</td>
		<td>
		<a href="https://github.com/brianfrankcooper/YCSB">[源码github]</a>
		</br>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
		</td>
		<td>离线数据批量入库性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
	</tr>
				
</tr>

<!-- 如下是Spark2X部分 -->
<tr>
<td rowspan=3 ><img class="navbar-logo" src="http://spark.apache.org/images/spark-logo-trademark.png"><i aria-hidden="true"></i></br>Spark2X</td>
		<td>HiBench</td>
		<td>
		<a href="https://github.com/hortonworks/hive-testbench">[源码github]</a>
		</br>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
		</td>
		<td>HadoopWordCount性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>

	<tr>
		<td>TPC-DS</td>
		<td>
		<a href="https://github.com/brianfrankcooper/YCSB">[源码github]</a>
		</br>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
		</td>
		<td>通用SQL查询测试</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
	</tr>
	
		<tr>
		<td>StructuredStreaming</td>
		<td>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
		</td>
		<td>流式查询性能测试</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
	</tr>
				
</tr>

<!-- 如下是Kafka部分 -->
<tr>
<td rowspan=1 ><img class="navbar-logo" src="https://cwiki.apache.org/confluence/download/attachments/27821302/KAFKA?version=2&modificationDate=1391968911000&api=v2"><i aria-hidden="true"></i></br>Kafka</td>
		<td>TPC-DS</td>
		<td>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
		</td>
		<td>生产、消费性能测试</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
</tr>


<!-- 如下是Storm部分 -->
<tr>
	<td rowspan=3 ><img class="navbar-logo" src="http://storm.apache.org/images/logo.png"><i aria-hidden="true"></i></br>Storm</td>
	<td rowspan=3 >HiBench6.0</td>
	<td rowspan=3 >
		<a href="https://github.com/hortonworks/hive-testbench">[源码github]</a>
		</br>
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
	</td>
		<td>WordCount模式性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		
		<tr>
		<td>fixwindow模式性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>

		<tr>
		<td>identity模式性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>

</tr>

<!-- 如下是Redis部分 -->
<tr>
	<td rowspan=3 ><img class="navbar-logo" src="http://www.redis.cn/images/redis-white.png"><i aria-hidden="true"></i></br>Redis</td>
	<td rowspan=3 >华为自研工具</td>
	<td rowspan=3 >
		<a href="https://github.com/linkedin/dynamometer">[FI源码github]</a>
	</td>
		<td>数据类型String读写性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		
		<tr>
		<td>数据类型Hash读写性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>

		<tr>
		<td>数据类型List读写性能</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		</tr>

</tr>

<!-- 如下是Flink部分 -->
<tr>
		<td rowspan=1 ><img class="navbar-logo" src="https://flink.apache.org/img/flink-header-logo.svg"><i aria-hidden="true"></i></br>Flink</td>
		<td>Streaming Benchmark</td>
		<td>
		<a href="https://github.com/hortonworks/hive-testbench">[源码github]</a>
		</td>
		<td>吞吐量、性能测试</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
</tr>

<!-- 如下是Solr部分 -->
<tr>
<td rowspan=1 ><img class="navbar-logo" src="https://cwiki.apache.org/confluence/download/attachments/120722742/SOLR?version=1&modificationDate=1561758170000&api=v2"><i aria-hidden="true"></i></br>Solr</td>
		<td>华为自研工具</td>
		<td>
		<a href="https://github.com/hortonworks/hive-testbench">[源码github]</a>
		</td>
		<td>入库、查询性能测试</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
</tr>

<!-- 如下是ElasticSearch部分 -->
<tr>
<td rowspan=1 ><img class="navbar-logo" src="https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=1678738792,678722178&fm=26&gp=0.jpg"><i aria-hidden="true"></i></br>ElasticSearch</td>
		<td>华为自研esarrayGA</td>
		<td>
		<a href="https://github.com/hortonworks/hive-testbench">[源码github]</a>
		</td>
		<td>入库、查询性能测试</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
		<td>
		<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
		</td>
</tr>

</table>