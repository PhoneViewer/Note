
 [回到目录](https://github.com/PhoneViewer/Note/blob/master/README.md)

## 利用adb无线连接android手机进行调式 无需获得root权限

### 1. 大部分设备

  输入adb devices查看我们连接的设备
  
  使用 adb tcpip 8888 设置端口号，5555为默认端口号，也可以设置其它端口号，端口号为需要为4位数
  
  拔掉我们的设备，开始无线连接 adb connect  
  
  使用adb connect 192.168.1.65:8888;
  
  192.168.1.65为我们手机的ip地址， 其中8888是我们自己设的端口号，这个端口号要和adb tcpip 设置的端口号保持一样;
  
  如果我们没有自己设置端口号，直接adb connect192.168.1.65就行了，默认使用5555。     
  
### 2. 部分设备

  输入 adb shell
  
  输入 setprop service.adb.tcp.port 5555  , 其中5555为默认端口号，也可以设置其它端口号，端口号为需要为4位数。 
  
  输入 stop adbd
  
  输入 start adbd
  
  最后 exit
  
### 3. 取消

  取消连接就是 adb disconnect  
  
  adb disconnect 192.168.1.65:8888
  
---------------------

本文来自 灵动的monkey 的CSDN 博客 ，全文地址请点击：https://blog.csdn.net/lnking1992/article/details/53465183?utm_source=copy 
