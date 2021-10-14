# 串口通信

## 串口接线

1. ID2000自带DB9串口接头，无需手动接线
2. ID3000 需要手动连接读码器的RX、TX、GND
3. ID5000 需要手动连接读码器的RX、TX、GND

![](<../.gitbook/assets/image (32).png>)

![](<../.gitbook/assets/image (33).png>)

### 常用的 9-pin 公头 232 串口连接器串口头定义如图

![](<../.gitbook/assets/image (55).png>)

![](<../.gitbook/assets/image (56).png>)

![设备 232 接口与其他带 232 串口的外部设备的接线](<../.gitbook/assets/image (57).png>)

### 读码器通信协议选择Serial，设置波特率等参数

![](<../.gitbook/assets/image (35).png>)

![](<../.gitbook/assets/image (36).png>)

最后，使用串口助手发送触发指令，检查是否能触发读码器工作即可

![](<../.gitbook/assets/image (37).png>)



## 常见问题

Q：读到码后串口没有数据输出 

A：需要把读码器设置为Normal模式，格式化标识符添加



Q：串口输出了与条码无关的调试信息 

A：需要更新到最新版固件才能屏蔽调试信息



Q：相机上电时会打印开机信息 

A：暂时无法屏蔽该信息
