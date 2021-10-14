# TCP触发

![触发模式选择TCP](<../.gitbook/assets/image (83).png>)

读码器TCP触发的时候， 读码器是作为TCP server的，所以我们要用TCP client 发送指令给读码器进行触发。

首先查看读码器的IP地址

![ip地址](<../.gitbook/assets/image (84).png>)

使用网络调试助手，作为TCP client 填写读码器的ip、端口

![调试助手](<../.gitbook/assets/image (85).png>)

设置读码器数据输出方式（本次测试使用TCP server，实际使用也可以选其他方式）

![](<../.gitbook/assets/image (86).png>)

设置数据读码器输出格式

![输出格式符选择条码内容code content ](<../.gitbook/assets/image (87).png>)

最后，IDMVS点击开始采集按钮，TCP调试助手发送触发指令，即可触发相机读码

![](<../.gitbook/assets/image (88).png>)

![](<../.gitbook/assets/image (89).png>)

可以看到发送start指令后，可以触发，并且收到读码结果。

