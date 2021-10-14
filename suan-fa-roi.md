---
description: 算法 ROI 可以只对设备选定的感兴趣区域进行算法识别，其他区域不做算法处理，提高读码效率。
---

# 算法ROI

> 算法 ROI 可以只对设备选定的感兴趣区域进行算法识别，其他区域不做算法处理，提高读码效率。
>
> 可设置多个算法 ROI 区域，并按照条码所在算法 ROI 区域的编号由 小到大排序输出条码结果。输出规则如下： 1：条码 2：条码 3：条码……
>
> 若某算法 ROI 区域内未识别到条码，则相应区域的条码信息更改为设置的 noread 字符。
>
>

### 手动绘制ROI

1、IDMVS连接读码器，test模式、触发关闭的状态下预览一次，确保图像出现，然后停止预览

![](<.gitbook/assets/image (146).png>)



2、点击“算法配置”模块右上角“所有属性”，找到算法 ROI 参数。

![](<.gitbook/assets/image (147).png>)

![](<.gitbook/assets/image (148).png>)

3、选择绘制的ROI序号，这里以Region1（ROI1）为例，再点击“绘制”，此时鼠标在预览窗口变为十字，拖动鼠标可出现绿色的框。

![](<.gitbook/assets/image (149).png>)

根据实际需求调整绿色窗口的大小和位置，此时被框选部分被设置为算法感兴趣区域，ROI以外的不读码

![](<.gitbook/assets/image (150).png>)

![](<.gitbook/assets/image (151).png>)

4、读码器支持多个ROI，我们用同样的步骤选择Region2 

![](<.gitbook/assets/image (152).png>)

如果想让读码结果包含ROI序号，可以在数据处理里添加ROI号（我们此处以TCP通信为例）

![](<.gitbook/assets/image (153).png>)

![](<.gitbook/assets/image (154).png>)



