# IO触发参数详解

![IO触发参数](<../../.gitbook/assets/image (71).png>)

#### Trigger Mode

* On：触发模式使能
* Off：关闭触发模式

#### Trigger In Source

* LineIn 0：0号输入管脚
* LineIn 1：1号输入管脚
* LineIn2：2号输入管脚
* 注意ID2000比较特殊，还拥有LineIn3：3号输入管脚；LineIn 0/1/2/3还需要手动配置为输入/输出

#### Debounce Time：防抖时间（单位：us，1000us=1ms=0.001s），对输入的触发信号进行去抖处理

* 当设置的去抖时间大于触发信号脉宽时，则该触发信号被忽略
* 当设置的去抖时间小于触发信号脉宽时，则该触发信号有效，注意，触发信号会被延迟后输出

![防抖时间原理图](<../../.gitbook/assets/image (72).png>)

#### Trigger In Polarity：IO触发方式

* Rising Edge：外部设备给出的电平信号在上升沿时，设备接收触发信号开始采图
* Falling Edge：外部设备给出的电平信号在下降沿时，设备接收触发信号开始采图
* Level High：外部设备给出的电平信号在高电平时， 设备一直处于图像采集状态
* Level Low：外部设备给出的电平信号在低电平时， 设备一直处于图像采集状态

![](<../../.gitbook/assets/image (73).png>)



#### Trigger Delay：触发延时时间（单位：us，1000us=1ms=0.001s）

* 使用Rising Edge 或 Falling Edge时，该参数生效

![](<../../.gitbook/assets/image (74).png>)

#### Start Delay Time：触发电平的的上升沿延时（单位：us）

* 使用Level High/Level Low时，该参数生效

#### End Delay Time：触发电平的的下降沿延时（单位：us）

* 使用Level High/Level Low时，该参数生效

![](<../../.gitbook/assets/image (75).png>)

如图所示： 

t1 是电平的上升沿延时，对于 Start Delay Time(us)

 t2 是电平的下降沿延时，对于 End Delay Time(us) 使用时候，需保证 t2 >= t1

#### Trigger Cache：触发缓存（仅部分读码器有这个功能）

开启后在触发过程若接收到新的触发信号， 可将该信号保留并进行处理。

* 不启用触发缓存使能： 强制结束第 1 个触发信号处理过程，开始处理第 2 个触 发信号

![第 1 帧被强制结束时序](<../../.gitbook/assets/image (76).png>)

* 启用触发缓存使能：前 1 个触发不会被强制结束，待处理完再进行第2次触发

![](<../../.gitbook/assets/image (77).png>)







