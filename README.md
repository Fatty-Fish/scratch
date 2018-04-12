# scratch
刮奖（会中哦）

#### 技术
H5 canvas 绘图

#### 效果gif图
<img src = "https://github.com/Fatty-Fish/scratch/raw/master/1.gif" height = "300px"/></br>

#### 思路

用了两个 canvas 画布。第一个，用于画出背景：狗狗图片和文字“恭喜你，中奖了！”。第二个，用于遮住背景和擦掉遮挡画布。
第二个画布用到 canvas 对象的 globalCompositeOperation 属性。
我用的 destination-out ：在源图像外显示目标图像。只有源图像外的目标图像部分会被显示，源图像是透明的。
动态创建源图像，源图像是以鼠标坐标为圆心，半径20的圆。

##### globalCompositeOperation
globalCompositeOperation 属性设置或返回如何将一个源（新的）图像绘制到目标（已有）的图像上。
源图像 = 打算放置到画布上的绘图。
目标图像 = 已经放置在画布上的绘图。
