# 数据处理

设备可通过“数据处理”模块对设备的过滤规则和输出数据处理进行设置。

### 过滤规则

* 普通过滤模式：通过IDMVS界面直观设置（按特定字符开头、结尾等简单过滤）
* 正则表达式过滤：可以根据正则表达式对读到的码进行过滤

![](<../.gitbook/assets/image (93).png>)

* 读取次数阈值： 当同一个条码读取结果相同的次数超过该数值时，认为此为有效条 码且输出结果； 当低于该数值时，则认为此为无效条码且不输出结果。

### 数据处理

数据处理部分可以对设备输出的条码结果进行设置。选择的通信协议不同，具体参数 内容有所差别。

* 排序规则：可根据实际需求选择输出结果的排序规则，支持多种排序规则
  * ROI ASC：按照ROI升序排列
  * ROI DESC：按照ROI降序排列
  * Center Coordinate X ASC：按照条码坐标X轴方向升序排列
  * Center Coordinate X DESC：按照条码坐标X轴方向降序排列
  * Center Coordinate Y ASC：按照条码坐标Y轴方向升序排列
  * Center Coordinate Y DESC：按照条码坐标Y轴方向降序排列
  * Scan ASC：按照扫码顺序升序排列
  * Scan DESC：按照扫码顺序降序排列
  * Code Type ASC：
  * Code Type DESC：
  * Code Length ASC：
  * Code Length DESC：

![](<../.gitbook/assets/image (95).png>)



* ROI 无读补齐： ROI Noread 补齐开关，输出的条码根据所在 ROI 区域的索引号排序输 出，在条码前添加 ROI 区域索引号，未读到码的区域自动补成 Noread。
* 输出格式化标志符添加： 点击右侧的”+“ 选择数据格式化的内容，可多选。

![](<../.gitbook/assets/image (96).png>)

* 输出开始：传输数据中开始部分的内容，可根据实际需求设置特定的内容。
* 输出结束：传输数据中结束部分的内容，可根据实际需求设置特定的内容。
* 输出条码输入字符使能：传输数据中结束部分的内容添加回车符（\r, 0x0d）
* 输出条码换行符使能：传输数据中结束部分的内容添加换行符（\n, 0x0a）

