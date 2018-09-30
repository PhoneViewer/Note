 [回到目录](https://github.com/PhoneViewer/Note/blob/master/README.md)
 
 ### android adb 查看ip地址命令
 
 要获取Android设备的IP地址，必须先保证:

1.你的Android设备已经连接到无线网络（此处的无线网络包括WiFi和WAPI，不包括3G或2G的移动网络）。

2.已连接到你的Android设备，即adb devices可以发现设备
 
~~先执行命令：adb shell netcfg~~

再执行命令：adb shell ifconfig eth0

---------------------

本文来自 liuhongxiangm 的CSDN 博客 ，全文地址请点击：https://blog.csdn.net/liuhongxiangm/article/details/27171201?utm_source=copy 
