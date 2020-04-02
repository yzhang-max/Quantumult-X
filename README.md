#  详细配置请查看作者github 文档  https://github.com/crossutility

## Quantumult X 使用教程:[链接](https://www.notion.so/kopshawn/Quantumult-X-1d32ddc6e61c4892ad2ec5ea47f00917)
## 神机规则:[链接](https://github.com/ConnersHua/Profiles/tree/master#%E4%B8%93%E4%B8%9A%E7%89%88)

## 本地/iCloud 文件夹挂载实现 Github 脚本库实时同步[教程](https://www.notion.so/github-948f19e65e1a47b3b468451491a3f34b)


## 五位 Cron 测试 https://tool.lu/crontab/

-----------------------------------------

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


----------------------------------------------------


神机规则：https://github.com/ConnersHua/Profiles/tree/master 
逗比规则：https://github.com/tudi1909/Surge_iOS_Rules 
lhie1规则：https://github.com/lhie1/Rules/tree/master 
nzw9314脚本库: github.com/nzw9314/QuantumultX/tree/master
chavyleung脚本库:https://github.com/chavyleung/scripts
NobyDa野比脚本库:https://github.com/NobyDa/Script.git



……............


---------------------------------------------------
#Tips

Quantumult X 格式节点转换

- SSR / SS 订阅可直接使用，无需转换，但你仍旧可以使用 API 来定制需求（节点过滤，开启 UDP / TFO 等等）
- V2RayN 链接，需要转换成 Quantumult X 格式后导入使用

1️⃣  在线转换API：
隐私问题，自行考虑
- https://sub.dleris.best/
- https://web.api.ytoo-163cdn.com
- https://bianyuan.xyz/
- https://gfwsb.114514.best/
更多定制参数（emoji，排序，重命名等）可参考 以下 API
- https://github.com/KOP-XIAO/QuantumultX-Surge-API
- https://github.com/tindy2013/subconverter 
获取最终链接后，填入 Quantumult X 的 ”节点 / 引用“ 即可订阅

2️⃣ iOS13 可用捷径：
V2rayN 订阅转换：
- https://www.icloud.com/shortcuts/cdd06a4537744ae3be7add425da95f6a
单条 V2 链接转换：
- https://www.icloud.com/shortcuts/89d5edee8dd944749f88f930aa9ad587
转换后手动填入 Quantumult X 配置文件（[server_local] 模块）


