# 输出参数详解

设备光耦输出信号，可用于控制 PLC、闪光灯、喇叭以及传感器等外部设备。

输出部分需配置设备的输出端口以及输出事件，并可设置输出反转功能（高电平变低电平，低电平变高电平）

![输出参数](<../.gitbook/assets/image (78).png>)

### Line Out Selector：选择输出端口（lineout0/1/2，ID2000还有一个lineout3）

### Line Out Inverter：输出电平反转

### Line Out Activation Event：输出事件处根据实际使用需求下拉选择对应的事件源， 设备会根据选择的事件源输出电平信号（仅介绍最常用的几种）。

* Off：无事件源，输出信号不变
* NoCodeRead：没读到码的时候输出信号，可以设置输出延时时间和持续时间
* ReadSuccess：读到码的时候输出信号，可以设置输出延时时间和持续时间
* LightStorbeLong：开始采集时输出信号，采集的时候就一直输出信号，不需要设置时间
* 当选择NoCodeRead或者ReadSuccess时，需要把Line Out Cache（触发缓存）关闭；

![](<../.gitbook/assets/image (79).png>)





###
