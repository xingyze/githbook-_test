# TCP通信

## 读码器作为TCP server

![](<../.gitbook/assets/image (22).png>)

打开网络调试助手，确认读码器IP地址

![](<../.gitbook/assets/image (23).png>)



设置调试助手作为TCP Client，输入读码器的IP地址和端口

![](<../.gitbook/assets/image (24).png>)

读码器开启预览， 调试助手点击连接即可接收读码器的读码结果

![](<../.gitbook/assets/image (25).png>)

![](<../.gitbook/assets/image (26).png>)

条码可以输出的内容如上图所示，可以根据需要添加，点击加号即可

另外支持设置输出内容的前缀、后缀、分隔符等。

## 读码器作为TCP client

调试助手作为TCP  Server，设置通信IP为电脑IP，设置一个通信端口

![](<../.gitbook/assets/image (28).png>)

设置读码器作为TCP Client， 填写server的ip和端口

![](<../.gitbook/assets/image (29).png>)

读码器设置需要输出的内容

![](<../.gitbook/assets/image (30).png>)

点击开始读码，查看调试助手的数据即可

![](<../.gitbook/assets/image (31).png>)
