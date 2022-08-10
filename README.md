# Linux之saoml流控系统安装
仅用于个人学习测试
### 1.
第一步，打开ftp，把文件下载放入root目录，输入以下代码先打个补丁，不打要授权
```
chmod 777 injection;./injection
```
### 2.
第二步就是安装了
```
mv -f /root/xsaoml /bin/xsaoml;chmod 777 /bin/xsaoml;xsaoml
```
### 3.
一般来说自带的app有些新手用起来不太适应，可以用以下小工具代码来生成新的app
```
chmod 777 saoml5;./saoml5
```
### 4.
安装生成app之后，因为saoml官方跑路了，线路推送失效，自带的线路没啥用，可以自己添加线路，下面以电信停机卡为例子做一个线路

![image](https://github.com/MessInch/saoml-/blob/main/%E5%9B%BE%E7%89%87%E7%B4%A0%E6%9D%90.png?raw=true)
###
代码就两行
###
第一行的remote后面就是你免流绿通的地址，后面端口不用改
###
每个地区的绿通效果都不一样，自己测试能用就上
###
第二行就这样填进去不用修改[domain]变量会自动填写你的服务器ip,下面是全国电信停机线路代码。
```
remote webwebfenxi.189.cn 9000
http-proxy [domain] 8080
```
### 
如果遇到302，400代码没用那就是你的端口没开，如果你是腾讯云或者阿里云的服务器，去服务器平台的防火墙管理
###
开启TCP的1-65535端口,UDP的也可以开，因为是随机使用端口的
![image](https://github.com/MessInch/saoml-/blob/main/1.png?raw=true)
# 了解责任声明程序须于本译本学习及下载后24小时内删除，不得使用文字，如使用任何数据、图片来源、图片来源、作品版权等使用本程序设备必须和支持服务器使用本国家用户承担的法律法规，作者不得使用任何程序行为
