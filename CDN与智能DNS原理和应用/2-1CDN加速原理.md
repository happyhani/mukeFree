###Welcome to use MarkDown
# CDN加速原理
## 内容缓存
* squid作为web服务，或其他Apache、 Ngix等均可。注： 如果内存有数据，直接返回客户端，如果没有，再去抓取一份数据再返回给客户端。
* 内容缓存到内存和本地文件。注：内存不够时，可以存放在本地文件中。比较热的数据放在缓存中，比较冷的数据放在本地文件中。
* 页面访问速度极高。 不需要都去源站访问。如果都去源站访问，那源站的访问带宽和处理性能都会产生瓶颈
## 分布在全国各地的网络节点
* 全国近百个城市，几百个服务器节点是很正常的
* 迅雷星域属于流量共享模式，上百万个节点。普通用户可以将自己的流量共享出去。
## 多线路支持
* 我国特点：南电信北联通
* 同时支持电信、联通、网通 等多种线路
* 不同于双线机房的双线接入        注： 自己维护的时候：一套系统使用双机房，双线（如联通电信）接入。成本高
* 减少跨网访问。 电信用户就用电信网络的访问 
## 适用范围
* 静态和更新频率低的内容更适用
* 数据流量大的产品更适用 （视频、直播、大量图片）
* 带宽价格更便宜  注：购买一个双线机房 1M带宽需要几十块。使用CDN的话，贵的几块，便宜的不到1块
# 3-1 CDN的具体使用
* 1、DNS解析换到CDN服务所提供的DNS解析上去
* 2、在CDN的后台里做相应的配置
## 管理功能
* 这里使用360云加速
* 预缓存
* 文件刷新 (主要使用)
* 目录刷新 (主要使用)
* 统计功能（图表统计）  注： cdn节点越多，命中率会低一点，因为会有更新的，有过期的








