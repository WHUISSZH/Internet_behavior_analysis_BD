# internet_behavior_project（大数据项目之用户上网行为分析）

## 项目

1.用途

用户上网行为分析

2.相关链接

[公众号链接](https://mp.weixin.qq.com/s/lkT29by8hmOzKq3Kaogg8Q)

[阿b直播录屏链接](https://www.bilibili.com/video/BV1Bt4y1G7z2/?spm_id_from=333.788&vd_source=d1c25b995c7a4d3fad25149c20815d5c)

## 期望
大数据入门项目，希望能理解熟悉从数据采集、清洗、处理、入库、利用的一系列流程和对应工具
 
## 数据源
1.如何获取数据

邮箱发issue，我把链接发你。

2.数据详情

1亿条真实的互联网用户上网数据，有非常规整的9个字段(我都替你清洗过了)，为了方便你们读取，我把它导出成CSV文件，其中第一行是schema。其字段意义解释分别如下：

client_ip: 指上网用户的ip地址，你可以根据这个ip知道这个用户大概的位置信息，这个有专门的api可以查询；

domain：指上网人要上的网站地址，你可以根据该网站的性质来判断这个人的上网行为；

time：上网人的上网时间；

target_ip: 上网人要上的网站的目标ip地址；

rcode：网站返回状态码，0为正常响应，2为不正常；

query_type: 查询类型，几乎都是1，即正常上网行为；

authority_recode：网站服务器真正返回的域名，可能跟domain不一样，如果不一样的话，可能说明是个钓鱼网站之类的，你可以去分析分析；

add_msg: 附加信息，几乎都为空，你可以看看如果有内容的话，到底是什么玩意；

dns_ip：当前要上的这个网站由哪个DNS服务器给提供的解析，一般一个DNS服务器会服务一个区域，如果由同一个DNS服务器进行解析的，说明他们在同一片大的区域；

以上是对这份数据的字段解读，相信从这些解释中，你已经大概能了解这份数据的作用了。
