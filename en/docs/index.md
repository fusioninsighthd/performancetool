
<!-- ex_nonav -->

# FusionInsight HD测试工具汇总

华为FusionInsight HD支持开源标准的Hadoop接口，兼容开源的Hadoop测试工具，因部分开源工具未考虑安全认证，故给出开源工具适配华为FI HD集群的测试操作指导！

<table class="tg">
 <thead>
 <tr>
  <td colspan=4 >测试工具</td>
  <td colspan=4>FusionInsight</td>
 </tr>
 <tr>
  <td rowspan=2><i aria-hidden="true">组件名称</td>
  <td rowspan=2><i aria-hidden="true">工具名称</td>
  <td rowspan=2><i aria-hidden="true">测试场景</td>
  <td rowspan=2><i aria-hidden="true">工具介绍及下载</td>
  <td rowspan=1 colspan=2><i aria-hidden="true">8.0</td>
  <td rowspan=1 colspan=2><i aria-hidden="true">6.5.1</td>
 </tr>
 <tr>
 <td>安全集群</td>
 <td>普通集群</td>
 <td>安全集群</td>
 <td>普通集群</td>
 </tr>
</thead>

<tr>

<td rowspan=5 ><img class="navbar-logo" src="/images/elephant.png"><i aria-hidden="true"></i></br>HDFS</td>
<td rowspan=4 ><i aria-hidden="true">TestDFSIO</td>
<td>NameNode随机写性能</td>
<td></td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
<tr>
<td>NameNode随机读性能</td>
<td></td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
</tr>
<tr>
<td>DataNode随机写性能</td>
<td></td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
</tr>
<tr>
<td>DataNode随机读性能</td>
<td></td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
</tr>
</tr>

<tr>
<td rowspan=1 >Dynamometer</td>
<td></td>
<td>
<a href="https://github.com/linkedin/dynamometer">github</a>
</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>

<tr>
<td rowspan=4 ><img class="navbar-logo" src="/images/elephant.png"><i aria-hidden="true"></i></br>Yarn</td>
<td rowspan=4 ><i aria-hidden="true">HiBench6.0</td>
<td>TeraSort</td>
<td></td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
</tr>

</tr>
<tr>
<td>WordCount</td>
<td></td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
</tr>
</tr>

</tr>
<tr>
<td>DataNode随机读性能</td>
<td></td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
</tr>
</tr>

</tr>
<tr>
<td>DataNode随机读性能</td>
<td></td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_Sec"><span class="label label-Pass ">操作指导</span></a>
</td>
<td>
<a href="Hive/TPC-DS_2.4_UnSec"><span class="label label-UnCheck ">未验证</span></a>
</td>
</tr>
</tr>


</table>