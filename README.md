
## Quantumult X 使用教程:[链接](https://www.notion.so/kopshawn/Quantumult-X-1d32ddc6e61c4892ad2ec5ea47f00917)
## 神机规则:[链接](https://github.com/ConnersHua/Profiles/tree/master#%E4%B8%93%E4%B8%9A%E7%89%88)

## 本地/iCloud 文件夹挂载实现 Github 脚本库实时同步[教程](https://www.notion.so/github-948f19e65e1a47b3b468451491a3f34b)

--------

# URL 方案示例

Formats of Quantumult X URL.

## API
- [quantumult-x:///update-configuration?remote-resource=url-encoded-json](https://github.com/crossutility/Quantumult-X)

``` text
quantumult-x:///update-configuration?remote-resource=%7B%0A%20%20%20%20%22server_remote%22%3A%20%5B%0A%20%20%20%20%20%20%20%20%22https%3A%2F%2Fraw.githubusercontent.com%2Fcrossutility%2FQuantumult-X%2Fmaster%2Fserver.txt%2C%20tag%3DSample-01%22%2C%0A%20%20%20%20%20%20%20%20%22https%3A%2F%2Fraw.githubusercontent.com%2Fcrossutility%2FQuantumult-X%2Fmaster%2Fserver-complete.txt%2C%20tag%3DSample-02%22%0A%20%20%20%20%5D%2C%0A%20%20%20%20%22filter_remote%22%3A%20%5B%0A%20%20%20%20%20%20%20%20%22https%3A%2F%2Fraw.githubusercontent.com%2Fcrossutility%2FQuantumult-X%2Fmaster%2Ffilter.txt%2C%20tag%3DSample%2C%20force-policy%3Dyour-policy-name%22%0A%20%20%20%20%5D%2C%0A%20%20%20%20%22rewrite_remote%22%3A%20%5B%0A%20%20%20%20%20%20%20%20%22https%3A%2F%2Fraw.githubusercontent.com%2Fcrossutility%2FQuantumult-X%2Fmaster%2Fsample-import-rewrite.txt%2C%20tag%3DSample%22%0A%20%20%20%20%5D%0A%7D
```
``` json
{
    "server_remote": [
        "https://raw.githubusercontent.com/crossutility/Quantumult-X/master/server.txt, tag=Sample-01", 
        "https://raw.githubusercontent.com/crossutility/Quantumult-X/master/server-complete.txt, tag=Sample-02"
    ],//订阅节点
    "filter_remote": [
        "https://raw.githubusercontent.com/crossutility/Quantumult-X/master/filter.txt, tag=Sample, force-policy=your-policy-name"
    ], //过滤规则
    "rewrite_remote": [
        "https://raw.githubusercontent.com/crossutility/Quantumult-X/master/sample-import-rewrite.txt, tag=Sample"
    ]  //复写规则
}
```


-----


提问（进群）先看置顶#FAQ (更新于2020-02-23)        

此群是【非官方群】，主要就Quantumult(X) 使用进行讨论。(开车会被ban，不讨论价值观等)，提问最好带截图/视频，不要一句 "不行/不能/用不了"。

Quantumult是一款iOS APP，下载地址（非国区）：https://appsto.re/us/o1dOkb.i
QauntumultX 是作者重构的另外一个 APP，也已经上架
（因为黑卡问题，在美国区商店暂时下架，建议港区、日区购买安装）。
App Store地址(港区):https://apps.apple.com/hk/app/quantumult-x/id1443988620
单独售价: 58 HKD, 7.99美刀
套餐https://apps.apple.com/hk/app-bundle/quantumult-x-upgrade/id1482985563
（限时免费更新已过，从quantumult 更新需付费20 HKD, 3美刀）
--------------------------------
Q：我不会用啊？有教程么？
A：如果有相关APP如Surge、Shadowrocket使用经验，阅读一下非官方使用手册（具体规则地址以 https://t.me/quantumultappnews/161 为准）：
- Quantumult 完整教程: https://github.com/shigalin/Quantumult/blob/master/README.md
- QuantumultX 用户教程: https://www.notion.so/kopshawn/Quantumult-X-1d32ddc6e61c4892ad2ec5ea47f00917
- 如果你是老手，自行参考 APP 内 示范配置，或者作者 github 文档：https://github.com/crossutility

Q：群里讨论的功能我为啥没有？如何申请TF？
A：可能是讨论quantumult(X)的TF版（即测试版），建议追求新功能的申请TF，除非商店版bug影响正常使用（TF版也可能有新的bug）。发送邮件（带购买凭证）到 support@quantumult.crossutility.com 即可。

Q：购买凭证是什么？申请之后过多久可以收到TF？
A：购买APP后苹果发送的邮件，截图即可，可对自己的地址之类的敏感信息打码。
      TF通过时间不固定。

Q：我想对软件提建议或反馈。
A：发邮件即可，地址在上面。

Q：总是自己断开连接。淘宝很卡，邮件有问题咋办？
A：现在没有该bug，如果有，请参考早期排查方法 https://t.me/quantumultappnews/78
A2：各种奇葩问题可以尝试去 更多/模块/ 选择 loopback （最新版本已默认此模式）

Q：Quantumult和其他APP哪个好？Quantumult跟Quantumult X 哪个好？
A：各有千秋。说谁好完全没意义，爱用哪个用哪个，不过多讨论。

Q：Quantumult(X)规则有哪些？怎么导入？
A1：quantumult 规则推荐 https://t.me/useConfig/144 ，基本操作：https://t.me/useConfig/134 （此频道完全一家之言，有明显的偏向性，更多规则请浏览GitHub）。
A2: 而鉴于QuantumultX的各种新特性，推荐使用神机规则：https://github.com/ConnersHua/Profiles/tree/master

Q：Quantumult(X)支持啥代理类型？
A1：Quantumult支持SS / SSR / HTTP(over TLS) / SOCKS 5(over TLS) / V2ray，不支持V2ray的KCP
A2：quantumultX支持 SS/SSR，V2ray(不支持 KCP) ，HTTP(over tls)

Q：支持服务器订阅吗？
A1：quantumult支持ssr/ss订阅，以及quantumult格式的 v2ray订阅，在设置-订阅里面导入即可。
* 由于v2ray订阅没有官方格式，除非订阅明确说明支持Quantumult，否则需要转换，填上   https://tgbot.lbyczf.com/v2rayN2quan?url=订阅链接&group=分组名&method=你的加密方式 
    （ 分组名不能直接填中文，建议写英文并前提将订阅链接进行urlencode转码：https://www.urlencoder.org/  ）;
* v2ray的URI转换成quantumult格式URI，可去下面两个网站:  
链接 1️⃣:  http://quan.eicky.com
链接 2️⃣:  https://fndroid.github.io/quantumult-vmess
其余转换方式参考（比如Surge托管转SS订阅）： 
https://fndroid.github.io/api_constructor/index.html
http://t.cn/EwiLSK6 。
【隐私问题自己考虑】

A2:QuantumultX支持一般格式的 ss/ssr 订阅，以及quanx格式的ss/ssr/v2订阅（具体格式参见APP内示范配置或者前面教程），
可尝试用各种第三方API转换，将通用的 ss/ssr/vmess/surge 等格式链接转换成 quanx 格式的订阅，
例如：https://github.com/KOP-XIAO/QuantumultX-Surge-API
【隐私问题自己考虑】
也可以使用此转换网站自助使用：https://gfwsb.114514.best

Q：自建SS订阅，格式是怎么样的？
A：https://t.me/useConfig/174

Q：如何隐藏状态栏VPN标记？
A：VPN标志隐藏开关:
QuantumultX：点右下角logo/其他设置(最下方)/0.0.0.0/31
Quantumult：更多/附加功能/Exclude Routers 0/31

隐藏功能（能点击点击，不能点击复制到浏览器打开）：
quantumult://
quantumult://start
quantumult://stop
quantumult://settings?toggle_vpn_status_icon（隐藏/显示VPN图标）
quantumult://settings?compatible_level=1
quantumult://settings?disable_http_proxy=on

为了避免造成不必要麻烦，看到新加群然后打广告的会删除广告内容。
机场太复杂，可以看看测评：https://www.duyaoss.com/index.php/archives/3/

看到无脑言论会忍不住warn（最终解释权归群主）
