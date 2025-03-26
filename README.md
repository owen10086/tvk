# 自动获取酒店源  组播源 #
## AQinTrue：https://github.com/AQinTrue/AQinTrue的提交一直不知道什么原因没有成功。参照大神的方法再一次修改了采用异步的方式优化网络请求，同时增加了异步线程。
## 自己使用时一定注意根据自己的网络情况修改800，830，873行的线程及时间。
## 不再依赖chrome浏览器及fofa等网站，windows系统可直接运行itvall.exe文件，大概45分钟。 ##
## 增加ZHGXTV的相关,ZHGXTV.exe可以在windows直接运行。 ##
### docker打包好的镜像可以在这里下载：### 
链接: https://pan.baidu.com/s/1NFv2K-uES0imKxG4XNh4fQ 提取码: 3s32

使用方法：

1.电视盒子

  在看电视直播软件中直接输入以下任一地址即可：
  
      https://ghproxy.net/https://raw.githubusercontent.com/ssili126/tv/main/itvlist.txt
      https://raw.githubusercontent.com/ssili126/tv/main/itvlist.txt
  
2.想自己获取电视直播地址的可采用以下方法：

  windows电脑：
  
      1.1 下载当前目录下的itvall.exe,
      1.2 运行完成后在当前目录下生成电视直播文件itvlist.txt。
  
  有安装python的电脑：
  
      2.1 下载new.py
      2.2 pip install requests futures eventlet
      2.3 运行new.py
      2.4 运行完成后在当前目录下生成电视直播文件itvlist.txt。

3.在openwrt或群辉的docker运行：

        1.安装：docker pull liuxipo/itvall:amd64  或者 docker pull liuxipo/itvall:arm64
        2.运行：docker run -v /www/itvall:/app itvall
        3.访问：http://本地ip/itvall/itvlist.txt
  
4.推荐在本地电脑运行，不推荐在github运行。github获得的数据不准确，测速不准。

5.udpxy目录为部分组播源。

