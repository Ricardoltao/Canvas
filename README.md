# Canvas

## canvas 绘制基础

### 画直线

canvas是以左上角为原点，上边为x，左边为y

我们可以通过 `moveTo(x,y)`，来移动需要从哪里开始绘制，即起点。用`lineTo(x,y)`，来绘制路径。以上只是把路径描述出来

需要配合`stroke()`和`fill()`来进行绘制：

+ stroke画线
+ fill填充颜色

如果需要对不同的区域设置不同的样式，需要结合`beginPath()` 和 `closePath`



### 绘制弧线

context.arc(centerx,centery,radius,startingAngle,endingAngle,anticlockwise=false)

+ startingAngle和endingAngle开始弧度值和结束弧度值
+ anticlockwise顺时针绘制还是逆时针