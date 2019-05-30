# canvas 知识点整理
canvas是一个可以使用脚本来绘制图形的HTML元素

## 基本用法
canvas只有两个属性width，height，默认大小300/150
+ 替换内容，<canvas>替换的标签或文字</canvas>
+ 渲染上下文  
使用getContext()方法获得渲染上下文。
+ 检查支持性

## 绘制形状
+ 栅格，左上角0，0，
+ 绘制矩形
	+ fillRect(x,y,width,height)绘制一个填充的矩形
	+ strokeRect(x,y,width,height)绘制一个矩形边框
	+ clearRect(x,y,width,height)清除指定矩形区域，完全透明
+ 绘制路径
	+ 创建路径起始点，画图，封闭路径，描边或填充
	+ beginPath()新建一条路径,图新绘制命令被指向到路径上，首先moveTo指定起始位置
	+ closePath()闭合路径之后图形绘制命令又重新指向到上下文中
	+ stroke()通过线条来绘制图形轮廓
	+ fill()通过填充路径的内容去区域生成实心的图形，会自动闭合  
	移动笔触moveTo(x,y)