本文是一个微成熟小白对于科学上网的一些切身感受的整理，自己捋思路，同时也为方便他人。顺便会不断更新一些实用资源、工具等。发现错误的地方欢迎斧正。正文中点击目录会跳转到相应内容，点标题也可快速返回目录位置。<br>
`2020年5月8日更新：新增tiktok最新破解版（iOS+Android）、酷我音乐破解版（Win+Android）、音乐间谍重制版（Windows）、spotify全功能破解版（Android）`<br>
* <a id="h1" href="#c1">一、国内网络基本了解 </a> <br>
* <a id="h2" href="#c2">二、科学上网 </a> <br>
  * <a id="h2.1" href="#c2.1">No1、没落的“VPN” </a> <br>
    * <a id="h2.1.1" href="#c2.1.1">什么是VPN </a>
    * <a id="h2.1.2" href="#c2.1.2">VPN现状 </a>
  * <a id="h2.2" href="#c2.2">No1、关于机场 </a> <br>
    * <a id="h2.2.1" href="#c2.2.1">什么是机场 </a>
    * <a id="h2.2.2" href="#c2.2.2">机场的选择 </a>
      * <a id="h2.2.2.1" href="#c2.2.2.1">技术层面 </a>
        * <a id="h2.2.2.1.1" href="#c2.2.2.1.1">BGP中转和IPLC的通俗理解 </a>
      * <a id="h2.2.2.2" href="#c2.2.2.2">主观层面 </a> 
        * <a id="h2.2.2.2.1" href="#c2.2.2.2.1">机场的外观设计 </a> 
        * <a id="h2.2.2.2.2" href="#c2.2.2.2.2">机场电报群观察交流 </a>
        * <a id="h2.2.2.2.3" href="#c2.2.2.2.3">机场的测速 </a>
        * <a id="h2.2.2.2.4" href="#c2.2.2.2.4">机场价格 </a>
* <a id="h3" href="#c3">三、我的机场推荐及使用感受 </a> <br>
  * <a id="h3.1" href="#c3.1">SSR、V2ray机场：STC </a> <br>
  * <a id="h3.2" href="#c3.2">Trojan机场 </a> <br>
  * <a id="h3.3" href="#c3.3">机场综合使用感受 </a> <br>
* <a id="h4" href="#c4">四、主流科学上网工具下载(包含Win、Mac、Android三大平台) </a> <br>
  * <a id="h4.1" href="#c4.1">V2ray(含官方使用手册) </a> <br>
  * <a id="h4.2" href="#c4.2">clash(含CFW使用说明书) </a> <br>
    * <a id="h4.2.1" href="#c4.2.1">ClashR汉化版，支持SSR和V2订阅 </a> <br>
  * <a id="h4.3" href="#c4.3">Trojan </a> <br> 
  * <a id="h4.4" href="#c4.4">SSTAP </a> <br>
  * <a id="h4.5" href="#c4.5">Netch(Win) </a> <br>
  * <a id="h4.6" href="#c4.6">Mellow </a> <br>
  * <a id="h4.7" href="#c4.7">Pharos Pro(Android) </a> <br>
  * <a id="h4.8" href="#c4.8">shadowrocket基础教程及分组规则自动切换节点 </a> <br>
  * <a id="h4.9" href="#c4.9">Shadowsocks </a> <br>
  * <a id="h4.10" href="#c4.10">ShadowsocksR </a> <br>
* <a id="h5" href="#c5">五、其它实用资源、工具 </a> <br>  
 
***

# <a id="c1" href="#h1">一、国内网络基本了解 </a> <br>
# 一、国内网络基本了解
大家都知道，我们中国对网络的限制比较严格，不是所有的网站咱们都能浏览。国家主要通过GFW([dns劫持](https://baike.baidu.com/item/%E5%9F%9F%E5%90%8D%E5%8A%AB%E6%8C%81/7657893?fromtitle=DNS%E5%8A%AB%E6%8C%81&fromid=6739044&fr=aladdin)、[dns污染](https://baike.baidu.com/item/DNS%E6%B1%A1%E6%9F%93)和[ip封锁](https://baike.baidu.com/item/ip%E5%B0%81%E9%94%81)等手段)进行网络封锁。下图是百度百科对GFW（俗称“墙”）的介绍
![GFW](https://www.louimg.com/u/20200312/11050110.png "GFW的介绍")
大家主要看红圈里的文字，GFW的功劳：让国民政治觉悟提升了不少，所以GFW只会越来越完善。但对于大多数网民来说，网络是我们学习、工作、美好生活的重要工具，GFW一定程度上把好多对我们学习、工作有帮助的综合性很强的技术、学术网站、社交网站等也拒之门外。
<br>大家经常听说的网站如[油管YouTube](https://www.youtube.com)、[脸书Facebook](https://www.facebook.com/)、[推特Twitter](https://twitter.com)、[电报telegram](https://telegram.org/)、[谷歌google](https://www.google.com.hk/)、[维基百科](https://zh.wikipedia.org/)等，这些我们都是无法正常访问的。需要科学上网（俗称翻墙）才能上。所以，这种背景下，也就出现了各种各样的突破GFW限制的工具，突破网络审查的软件通常被称作翻墙软件，俗称梯子。翻墙软件并不只是大家理解的VPN软件，还有基于其它协议的代理软件。<br>[回到顶部](#readme)
***

# 二、科学上网
## 没落的“VPN”
#### 1. 什么是VPN
VPN全称“虚拟私人网络（Virtual Private Network）”，VPN是一个统称。VPN是一种加密通讯技术，它被设计出来的目的是数据传输安全和网络匿名。所以它不是为了翻墙而生的，维基百科里关于VPN的介绍，说它的特殊使用才是翻墙。它的出现远早于GFW。
![VPN](https://www.louimg.com/u/20200312/15453995.png "VPN的维基介绍")
GFW机制加上劳动人民的无穷智慧，促使聪慧的劳动人民开始用VPN连接外国网络实现翻墙，随着使用人数的激增和网络环境的发展，商业化的一键VPN也逐渐成熟，一些免费VPN和付费VPN就这样诞生了。<br>[回到顶部](#readme)
#### 2. VPN现状
使用VPN，不足之处在于数据分流不灵活，会将开启了VPN的设备的所有数据流量全部导向至VPN服务器上；另外如果VPN服务器上有流量监视软件运行，那么用户所传输的数据将有信息安全威胁；进一步来说，由于VPN设计的初衷并不是用于翻墙，因此数据流量的特征非常明显，容易引起审查机构注意，导致被封。所以，VPN这种翻墙方式基本已经没落了。但是市场上还是有一些一键VPN软件，它们背后的原理其实已经背离了VPN的真正原理，这些一键VPN其实就是把一些机场节点融合到了自己的APP，所以现在好多得VPN其实也不算真正的VPN了。至于免费的VPN，由于用户人数与流量众多，常会暴露出了公共网络服务的特质，所以经常会被封，而且VPN也存在后台钓鱼的风险，虽然可能现在这种情况好多了（谁知道呢），但是之前毕竟存在过，所以本人主观上严重不建议长期使用这种一键VPN软件。<br>
VPN作为过去很长一段时间最主流最热门最常用最为人所知的翻墙手段，已然成为翻墙的代名词。即便是VPN已不再常用的今天，当人们谈及翻墙的时候，说得最多的仍是：“你有什么好用的vpn吗？”<br>
[回到顶部](#readme)<br>
***

## 关于[机场](https://t.co/OGzuQ1kAL3?amp=1)
### 1. 什么是[机场](https://t.co/OGzuQ1kAL3?amp=1)
随着VPN的没落，现在主流的科学上网方式是大家经常听的SS（Shadowsocks）、ssr（ShadowsocksR）、V2(v2ray)、Trojan等等这些代理工具，还有基于这些代理工具的原理，扩展衍生出的在各平台使用且支持以上几种翻墙协议的科学上网工具，如clash、Netch、shadowrocket、Quantumult、Pharos Pro等等非常多。<br>
这些工具的统一特点就是：工具自身没有翻墙功能，需要自行在服务端和客户端上部署，优点就是更加安全、速度更快，看似比一键VPN方法“繁琐”，但实际操作非常简单，其中服务端的部署有两种情况：<br>
第一种是我们自己购买vps部署，这就是人们常说的我自己搭建节点，喜欢折腾的伙伴可以自己去购买vps搭建，网上教程非常多，我自己是在谷歌云搭建了Trojan服务，具体教程本文第五部分有。<br>
第二种，就是有人替我们部署好了，直接用就可以。这也是目前用的最多的科学上网方式，提供这项服务的就是[机场](https://t.co/OGzuQ1kAL3?amp=1)。<br>
服务端部署好后，我们只需将服务器地址、端口这些基本信息添加到我们电脑或手机上的代理工具里，这就是客户端部署，这就实现了科学上网。现在很多工具都支持一键订阅，多数机场也提供了订阅链接，不需要我们手动逐一添加节点。<br>[回到顶部](#readme)
### 2. [机场](https://t.co/fdfliso9wM?amp=1)的选择
#### 技术层面
##### BGP中转和IPLC的通俗理解
大家在购买机场时候，会经常见到BGP中转、IPLC专线这些名词。至于他们的专业意义，自行google查询。对于很多不是专业研究这个的伙伴，就算我们查询了，也可能是似懂非懂的状态，所以这里不会给大家去深挖那些专业概念，我们尽量从小白角度出发，明白他们的所起的作用就行。<br>
首先，我们要了解的就是我们的电脑、手机通过机场翻墙，数据经历了一个什么过程，大致有以下几种类型（从专业角度讲，有些地方可能不是很恰当，但很形象）：
* 直连<br>
  * 用户 -> ss、ssr等协议 -> 公网传输穿过GFW -> 国外服务器<br>
大多数机场节点都是这种，尤其是一些免费节点。此方式成本低，因为是协议直接过GFW，虽然协议本身也做了技术处理，但大流量还是很容易被GFW识别，这也就是为什么有的机场节点经常会出现不稳定现象，或者干脆就被封不能用了。而且公网传输，使用人多，流量拥挤就会速度变慢。<br>
好点的机场主可能会单独购买一条线路，这也就是我们说的独享线路机场，速度还稍微快点。有些功利性的机场主会租一条线路，意味着这一条线路同时被租给N个机场，这是我们常说的共享线路机场，速度和稳定性就得碰运气了。<br>[回到顶部](#readme)
* 公网中转（BGP中转）<br>
  * 用户 -> ss、ssr等协议 -> 国内中转服务器 -> 公网穿过GFW ->  国外服务器<br>
中转服务器到GFW这一段，一般会使用一些隧道协议，以实现负载均衡、高可用、防止被墙等效果，且对传输速度也做了优化。但是加BGP中转是比较昂贵的，所以能发现机场中带BGP中转的节点价格会比普通节点的价格贵。
* 专线内网中转（IPLC）<br>
  * 用户 -> ss、ssr等协议 -> 专线服务器A（自带中转功能）-> 内网传输 -> 国外专线服务器B<br>
这种方式你会发现，少了一个环节，就是它没有过GFW，就是传说中的不会被墙，因为它压根就不过墙，而且是点对点直接传输，速度也是最快的。但是加IPLC比加BGP的价格更贵，所以你会发现，机场节点中带IPLC的也是卖的最贵的。目前国内大多的IPLC线都是采用的阿里内网线路，严格来说，不能算的上真正的IPLC。也有真正的IPLC线路，比较少，从商人角度来说，除非能回本儿，否则搞真正的IPLC是不划算的。<br>[回到顶部](#readme)
#### 主观层面
除了技术层面，我们选择一个机场就是靠我们的主观判断，我个人是从以下几个方面判断的，只能供大家参考，不是绝对正确，毕竟这个行业鱼龙混杂，只要不怕担风险，是个人就可以开机场去捞金，水也较深。<br>
##### 机场的外观设计
大家会发现，几乎所有机场的界面布局都长得差不多，那是因为99%的机场用的模板代码都是同一套代码，细心的话，进机场的网站，看右下角（一般在右下，也有可能在左下），都有个staff的标志，没有staff的，会有SSPANEL，点进去也会看到staff。所以怎么去设计更换更精美的皮肤，也能侧面反映出机场主的用心程度。
##### 机场电报群观察交流
大多数的机场都会提供电报群链接，机场主一般也会在里边，购买前可进电报群，肯定会有用过的人对机场的优点问题等进行交流，也可从机场主日常在群中的活跃程度、答疑解惑、日常交流等方面去感受一个机场主是否真正用心在建设这个机场。<br>[回到顶部](#readme)
##### 机场的测速
有些机场有试用，可试用测速。但个人建议测速的话，可以先尝试按流量去购买机场的服务，一般1G也就不到1元，管够测速使用了。这里建议测试分多个时间段去测，再把每个时间段的测速结果去做个平均，看是否满足你心理预期。多数人喜欢用YouTube测速，其实YouTube测速只能做个参考，想得到更精确的数据，还是用SPEEDTEST或FAST测，测速时候开启全局代理，把其它会走代理的程序全部关闭。
##### 机场价格
这个其实不好评判，因为每个人心理的标准都不一样，个人感觉，只要体验感和机场的价格对称就行。没有哪个贵，哪个便宜之说，都是相对的。要根据自己的实际需求去购买，这跟咱们平时买车一样，好车就是体验好，但价格也不便宜。<br>

综述，个人认为主观方面的判断有时候可能比技术层面更重要，机场速度再快，再稳定，如果一段时间就跑路了，那还是掉坑了，所以我更看重主观层面的判断。因我自己也买过跑路的机场，身边很多朋友、网友也跟我说被坑过，所以非常看重这方面。<br>[回到顶部](#readme)
# 三、我的[机场](https://t.co/OGzuQ1kAL3?amp=1)推荐及使用感受
## SSR、V2ray机场：STC，[官网](https://t.co/OGzuQ1kAL3?amp=1)
[STC机场](https://t.co/OGzuQ1kAL3?amp=1)，官网需要科学上网才能打开，用了将近一年半时间，我经历了三次机场升级，给我的体验感也由一般过渡到还行再到现在的好。也跟机场主聊过，去提一些建议，服务质量与价格还算对等。每次升级都是在大多客户反馈高峰期体验感不好的时候去考虑升级，去扩充升级一些设备，以带来更好的体验感。这也是**我看中的第一点**。毕竟它是从客户角度出发去考虑的，符合我上边说的主观层面判断，所以一直坚持用到现在。<br>
唯一可能不友好的一点就是价格也在随着升级在上涨，我觉得这个也可以理解，毕竟服务成本也在提高。**我看中的第二点**就是：涨价是不针对老客户的，就是你买了之后，不管以后机场涨价多少次，你永远都可用原来的价格去续费。还有，看YouTube4K视频、Netflix等视频网站没有任何问题。也可以去看一下[毒药大佬关于STC的测评](https://www.duyaoss.com/archives/1673/)。<br>
**STC机场支持订阅的工具如下图**
![stc订阅](https://www.nsaimg.com/2020/04/23/29e01443b25ec.jpg "stc订阅")
[回到顶部](#readme)
## Trojan机场：shadowsocks，[官网](https://t.co/FEE38PDhE6?amp=1)
官网需要科学上网才能打开，原来的老牌shadowsocks机场，在2020年2月份所有节点全部升级为Trojan，也是为了规避GFW，目前机场的名字还叫shadowsocks。这个机场我是从2015年开始使用，升级之后速度和稳定性都有了很大提升,下图是该机场在3月21日给客户发的邮件和我的购买账单，从服务升级到补差价，感觉也是从客户角度出发在考虑做更好的服务。<br>
![Trojan机场](https://www.louimg.com/u/20200323/15163186.jpg "Trojan机场")
![Trojan机场](https://www.louimg.com/u/20200329/10211993.png "Trojan机场")
**Trojan机场支持订阅的工具如下图**
![Trojan机场](https://www.nsaimg.com/2020/04/23/fb6508b7ece3e.jpg "Trojan机场")<br>
[回到顶部](#readme)
## 机场综合使用感受
* 我用的移动300M家用宽带，手机套餐免费送的宽带，平时翻墙会看Netflix和YouTube多点，而且经常会下载一些视频资源，两个机场配合使用完全能满足我的日常需求，用起来的区别就是：
  * 在一些晚高峰时段，[Trojan机场](https://t.co/FEE38PDhE6?amp=1)看YouTube4K偶尔会出现卡顿，但看1080P还是没什么问题的。[STC](https://t.co/OGzuQ1kAL3?amp=1)看4K完全不卡、但看8K偶尔也会出现卡顿。<br>
  * 下载视频时候，下载工具IDM，按照我的带宽，[STC](https://t.co/OGzuQ1kAL3?amp=1)是完全秒杀Trojan机场的，STC的下载速度平均下来能达到5M-10M不等,但[Trojan机场](https://t.co/FEE38PDhE6?amp=1)的下载速度平均下来只有1M-2M不等。<br>
  * 当然[STC](https://t.co/OGzuQ1kAL3?amp=1)的价格也比[Trojan机场](https://t.co/FEE38PDhE6?amp=1)的价格高出很多。[STC](https://t.co/OGzuQ1kAL3?amp=1)的基础套餐**每月38元**，还有其它的更高等级套餐，可自行到[STC官网](https://t.co/OGzuQ1kAL3?amp=1)查看。[Trojan机场](https://t.co/FEE38PDhE6?amp=1)的价格是`每年19.95AUD`（按现在汇率折合人民币86元）。价格标准请以机场官网最新价格为准。<br>
### 以上机场的使用教程见各自官网的帮助中心，各平台工具的配置步骤都非常详细。
  
[回到顶部](#readme)
***

# 四、主流科学上网工具下载(包含Win、Mac、Android三大平台)
`以下整理的工具大多都有详细的图文教程和GitHub下载地址，点详情可查看`<br>
`测试是否开启真正的全局代理的小方法，可供参考。打开你代理软件的全局代理模式，然后进入` https://www.ipip.net/ip.html `或` https://ip.cn/ `如果显示的IP地址是你所在地的IP，那么你还没实现真正的全局代理`
### V2ray（简称V2）

<details>
  <summary>详情</summary>
  支持VMESS协议的图形界面工具挺多的，下面给大家列举几个常用的<br>
  1、<a href="https://github.com/2dust/v2rayN/releases">V2ray的Windows端图形界面工具V2RayN下载</a>，V2rayN用的人挺多的，但好多
  人不知道，V2rayN要想真正实现全局代理，除了要右键选择“Http代理->开启Http代理，并自动配置系统代理（全局模式）”，还需要在参数设置里进行设置，具体看下
  图，顺便附上一个
  <a href="https://github.com/233boy/v2ray/wiki/V2RayN%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B">V2RayN详细图文教程。</a><br>
  <img src="https://www.nsaimg.com/2020/05/08/7843e43ebdf7d.jpg" alt="V2ray全局设置"><br>
  <img src="https://www.nsaimg.com/2020/05/08/a4f4786c141ee.jpg" alt="V2ray全局设置"><br>
  2、V2ray的Windows端图形界面工具<a href="https://github.com/Cenmrev/V2RayW/releases">V2RayW下载</a><br>
  3、V2ray的Mac端图形界面工具<a href="https://github.com/Cenmrev/V2RayX/releases">V2RayX下载</a>、
  <a href="https://github.com/yanue/V2rayU/releases">V2RayU下载</a><br>
  4、<a href="https://github.com/2dust/v2rayNG/releases">V2ray（Android）下载</a><br>
  5、<a href="https://www.v2ray.com/">V2ray官方使用手册文档</a><br>
</details>

### Clash

<details>
  <summary>详情</summary>
  1、clash也是一款不错的代理工具，支持VMESS和Trojan协议，但不支持ssr。它的衍生版clashR支持ssr、vmess协议。clash想要实现真正的全局代理，除了开启
  System Proxy外，还需要安装TAP虚拟网卡设备。<br>
  clash的Windows客户端叫做clash For Windows，简称CFW，<a href="https://github.com/Fndroid/clash_for_windows_pkg/releases">CFW下
  载。</a>给大家附上CFW的<a href="https://docs.cfw.lbyczf.com/">【文档教程】</a>和
  <a href="https://github.com/Shadowsocks-Wiki/shadowsocks/blob/master/zh_CN/v2ray/clash-for-windows-setup-guide.md">【图文教程】</a> 
  <br>
  2、<a href="https://github.com/yichengchen/clashX/releases">clash（Mac）下载</a><br>
  3、<a href="https://github.com/Kr328/ClashForAndroid/releases">clash（Android）下载</a>、
  <a href="https://play.google.com/store/apps/details?id=com.github.kr328.clash&hl=en_US">Clash in Google Play安装</a><br>
  4、<a href="https://474b.com/file/25713053-442345612">ClashR汉化版，支持SSR和V2ray订阅</a><br>
  5、<a href="https://docs.nameless13.com/shr/">ClashR各平台相关教程</a><br>
</details>

### Trojan

<details>
  <summary>详情</summary>
  1、支持Trojan协议的工具并不多，电脑端的图形界面工具有<a href="https://github.com/TheWanderingCoel/Trojan-Qt5/releases">Trojan-
  Qt5(Win+Mac+Linux)下载</a>，TrojanQt5支持一键订阅导入，只要你有Trojan机场订阅链接，即可一次性导入所有节点。工具界面如下图：<br>
  <img src="https://www.nsaimg.com/2020/05/08/7e444c1ec6dfb.png" alt="Trojan工具"><br>
  2、安卓端目前支持Trojan协议的工具<a href="https://github.com/trojan-gfw/igniter/releases">igniter下载</a><br>
  3、喜欢用黑屏命令风格的伙伴可下载<a href="https://github.com/trojan-gfw/trojan/releases">Trojan的Windows、macOS、Linux三大平台命令行工具
  </a><br>
  4、<a href="https://portal.shadowsocks.nl/knowledgebase/151/Trojan-%E6%9C%8D%E5%8A%A1%E5%AE%A2%E6%88%B7%E7%AB%AF%E8%AE%BE%E7%BD%AE%E6%95%99%E7%A8%8B%E7%B4%A2%E5%BC%95.html">以上Trojan工具的设置教程索引</a><br>
</details>

### Sstap

<details>
  <summary>详情</summary>
  1、真正的全局代理工具sstap，虽然是游戏加速器，但功能非常实用，通过专属虚拟网卡，真正实现系统内所有程序全部走代理，还可以根据自己需求选择内置代理
  DNS，让科学上网速度更快，安全性更高，具体见下图<br>
  <img src="https://www.nsaimg.com/2020/05/08/98abce621e6c5.jpg" alt="SSTAP">
  <img src="https://www.nsaimg.com/2020/05/08/6a7fd9ec22033.jpg" alt="SSTAP">
  2、<a href="https://474b.com/file/25713053-442234826">SSTAP下载</a><br>
</details>

### Netch

<details>
  <summary>详情</summary>
  1、Netch是一个开源游戏加速器。与需要添加规则以用作黑名单代理的SSTap不同，Netch更类似于SocksCap64，可以扫描需要代理的程序的安装目录，来专门获取其进程
  名称，从而实现真正分应用代理。 Netch也可以实现 SSTap那样的全局 TUN/TAP 代理。Netch现在支持Socks5，Shadowsocks，ShadowsocksR，VMess、Trojan协
  议，也是目前为数不多的几乎支持所有协议的工具。<br>
  <img src="https://www.nsaimg.com/2020/05/09/86fba7f8b2272.jpg" alt="netch">
  <img src="https://www.nsaimg.com/2020/05/09/39bc0a5b907f3.jpg" alt="netch">
  <img src="https://www.nsaimg.com/2020/05/09/3bb66a8cf22a7.jpg" alt="netch">
  2、<a href="https://github.com/NetchX/Netch/releases">Netch下载</a><br>
</details>

[回到顶部](#readme)

### Mellow

<details>
  <summary>详情</summary>
  1、Mellow 是一个基于规则的全局透明代理工具，可以运行在 Windows、macOS 和 Linux 上，也可以配置成路由器透明代理或代理网关，支持 SOCKS、HTTP、
  Shadowsocks、VMess 等多种代理协议。<br>
  2、<a href="https://github.com/mellow-io/mellow/releases">Mellow安装文件下载(Win+Mac+Linux)</a><br>
</details>

### Pharos Pro

<details>
  <summary>详情</summary>
  1、<a href="https://github.com/PharosVip/Pharos-Android-Test/releases">Pharos Pro(Android)下载</a><br>
  2、Pharos Pro(iOS)，登录非大陆AppleID下载，不会的可加电报群咨询我
</details>

### shadowrocket

<details>
  <summary>详情</summary>
  1、<a href="http://laob.me/2300/">ShadowRocket基础教程</a><br>
  2、<a href="https://blog.minirplus.com/14472/">ShadowRocket分组、规则自动切换节点</a><br>
</details>

### Shadowsocks（简称SS）

<details>
  <summary>详情</summary>
  1、<a href="https://github.com/shadowsocks/shadowsocks-windows/releases">Shadowsocks（Win）下载</a><br>
  2、<a href="https://github.com/shadowsocks/ShadowsocksX-NG/releases/">Shadowsocks（Mac）下载</a><br>
  3、<a href="https://github.com/shadowsocks/shadowsocks-android/releases">Shadowsocks（Android）下载</a><br>
</details>

### ShadowsocksR（简称SSR）

<details>
  <summary>详情</summary>
  1、<a href="https://github.com/shadowsocksrr/shadowsocksr-csharp/releases">ShadowsocksR（Win）下载</a><br>
  2、<a href="https://github.com/qinyuhang/ShadowsocksX-NG-R/releases">ShadowsocksR（Mac）下载</a><br>
  3、<a href="https://github.com/shadowsocksrr/shadowsocksr-android/releases">ShadowsocksR下载（Android）</a><br>
</details>

`关于iOS平台的科学上网工具，目前支持协议较完善的有shadowrocket、suerge、Quantumult、Pharos等，需要用非大陆AppleID下载且收费，请大家自行注册购买，不会的加群找我`

[回到顶部](#readme)
***

# 五、其它实用资源、工具
**有些资源需要提取码，加电报群即可获取提取码**
* [免费撸谷歌云300$搭建Trojan的全程记录](https://github.com/sxcool1024/googlecloud/blob/master/README.md)
* [著名摄影大师WANIMAL原版作品下载(已分享16.1G共8765张原图，持续更新中)](https://github.com/sxcool1024/WANIMAL-1983/blob/master/README.md)
* [机械工业出版社原版PDF电子书下载，提供当当网一键搜索查询(已分享2542册书籍，持续更新中)](https://github.com/sxcool1024/-Machinery-Industry-Press/blob/master/README.md)
* [《20世纪中华歌坛名人百集珍藏版合集》102张原版CD音轨](https://github.com/sxcool1024/20th-Century-Music)
* [周杰伦无损合集，发烧友正版碟片提取原版音轨](https://github.com/sxcool1024/Jay)

<details>
  <summary>Windows</summary>
  <a href="https://github.com/lyswhut/lx-music-desktop/releases">1、洛雪音乐助手桌面版官网</a><br>
  <a href="https://guihet.com/blackbird-player.html">2、黑鸟视频播放器官网（同时也是看电视直播节目利器，自带直播源）</a><br>
  <a href="https://474b.com/file/25713053-442341364">3、酷我音乐豪华破解版，支持无损下载</a><br>
  <a href="https://474b.com/file/25713053-442341369">4、音乐间谍重制版下载</a><br>
  <a href="http://t66y.com/index.php?u=297138&ext=e4669">5、草榴官网</a><br>
  <a href="https://474b.com/file/25713053-440658806">6、四十四个油猴脚本下载</a><br>
</details>

<details>
  <summary>Android</summary>
  <a href="http://www.wangdunwen.com/?inviteCode=ID3WVM">1、小小影视官网</a><br>
  <a href="https://www.wolong.tv">2、卧龙影视官网</a>    邀请码：WL345597<br>
  <a href="https://ng33.app/?channelCode=share?appkey=ayo1id&recommend=20965059">3、南瓜影视官网</a><br>
  <a href="https://dg77.app/?channelCode=share?appkey=zphsu3&recommend=4897090">4、冬瓜影视官网</a><br>
  <a href="https://474b.com/file/25713053-442341315">5、短信轰炸机永久使用版下载</a><br>
  <a href="https://474b.com/file/25713053-442341034">6、TikTok破解版下载</a><br>
  <a href="https://474b.com/file/25713053-442341207">7、酷我音乐破解版下载，支持无损</a><br>
  <a href="https://474b.com/file/25713053-442341313">8、spotify全功能破解版下载</a><br>
  <a href="https://github.com/yuuwill/1024app-android/releases">9、草榴APP下载</a><br>
  <a href="https://aff.91porn005.me/aff-afeFw">10、91app安装地址，不要通过扫码安装，安装地址复制到手机浏览器打开下载</a><br>
</details>

<details>
  <summary>iOS+Mac</summary>
  <a href="http://www.wangdunwen.com/?inviteCode=ID3WVM">1、小小影视官网</a><br>
  <a href="https://www.wolong.tv">2、卧龙影视官网</a>    邀请码：WL345597<br>
  <a href="https://ng33.app/?channelCode=share?appkey=ayo1id&recommend=20965059">3、南瓜影视官网</a><br>
  <a href="https://dg77.app/?channelCode=share?appkey=zphsu3&recommend=4897090">4、冬瓜影视官网</a><br>
  <a href="https://474b.com/file/25713053-442341476">5、TikTok苹果版下载</a><br>
  <a href="https://twitter.com/sxcool1024/status/1236090141606694912?s=20">6、iPhone快捷指令【下载YouTube、Twitter视频】</a><br>
  <a href="https://twitter.com/sxcool1024/status/1249974654325813248?s=20">7、iPhone快捷指令【举牌小人图片生成器】【文字转二维码】</a><br>
  
</details>

# 电报交流群：https://t.me/sxcool1024g
[回到顶部](#readme)



