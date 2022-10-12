# script-collect
收集一些不错的脚本，后面用来缝合怪

目前已收集脚本
1. Bypass_cdn （一款bypass cdn工具）

use eg:

```python3 .\scan.py https://www.ghxi.com/```

![image](https://user-images.githubusercontent.com/37091232/194805640-4fe2a74a-84de-4384-878a-2fa4c8083fda.png)


2. JSINFO-SCAN（JS信息搜集）

github地址：https://github.com/p1g3/JSINFO-SCAN

```python3 jsinfo.py -d jd.com --keyword jd --save jd.api.txt --savedomain jd.domain.txt```


（⭐）3. leakinfo_finder

自动爬取JS文件中接口，拼接接口，加入常见springboot等目录，进行http请求（get+post），正则匹配响应结果，输出敏感信息

github地址：https://github.com/Carrypan2022/leakinfo_finder

![image](https://user-images.githubusercontent.com/37091232/195039111-39f66975-09e8-4555-ae54-90a43f6fcad2.png)

希望增加：① url的响应状态码（js会有很多死链） ② 增加js中的正则匹配，以及提取接口的规则导出

4. py3zoomeye_subdomainapi

zoomeye钟馗之眼子域名查询api脚本，版本v2.0

github地址：https://github.com/moyuwa/zoomeye-subdomianapi

![image](https://user-images.githubusercontent.com/37091232/195241489-818ec188-26b7-4c32-aa14-ba718af3f2d8.png)
