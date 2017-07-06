## flex弹性盒
### 介绍  
弹性盒可以应用于响应式布局,是一种用于在页面上布置元素的布局模式，使得当页面布局必须适应不同的屏幕尺寸和显示设备时，元素可以预测的运行。他不使用浮动，flex容器的边缘也不会与其内容的边缘折叠。  
弹性布局是指通过调整其内元素的宽高，从而在任何显示设备上实现对可用显示空间最佳填充的能力。弹性容器扩展其内元素来填充可用空间，或将其收缩来避免溢出。	
### 弹性布局的相关词汇
![Alt text](flexbox.png)
<font color="red">(图片来自MDN)</font>  
1. 弹性容器(flex container)  
包含着弹性项目的父元素。通过设置 display 属性的值为 flex 或 inline-flex 来定义弹性容器。   
2.弹性项目(flex item)  
弹性容器的每个子元素都称为弹性项目。  
3. 轴(axis)  
每个弹性框布局包含两个轴。弹性项目沿其依次排列的那根轴称为主轴(main axis)。垂直于主轴的那根轴称为侧轴(cross axis)。  
<font color="blue">flex-direction</font>确定其主轴，其值主要有row|row-reverse|column|column-reverse，主要区别如图
![Alt text](flex-direction1.jpg)
<font color="blue">justify-content</font>性定义了浏览器如何分配顺着父容器主轴的弹性元素之间及其周围的空间。其值主要有flex-start | flex-end | center | space-between | space-around，主要区别 <a href="https://developer.mozilla.org/zh-CN/docs/Web/CSS/justify-content">看这里</a>  
<font color="blue">align-items</font> 定义了在当前行上，弹性项目沿侧轴默认如何排布。  
<font color="blue">align-self</font> 定义了单个弹性项目在侧轴上应当如何对齐，这个定义会覆盖由 align-items 所确立的默认值  
4. 方向(Direction)  
弹性容器的主轴起点(main start)/主轴终点(main end)和侧轴起点(cross start)/侧轴终点(cross end)描述了弹性项目排布的起点与终点。它们具体取决于弹性容器的主轴与侧轴中，由 writing-mode 确立的方向（从左到右、从右到左，等等）。  
<font color="blue">order</font> 属性将元素与序号关联起来，以此决定哪些元素先出现  
<font color="blue">flex-flow</font> 属性是 flex-direction 和 flex-wrap 属性的简写，决定弹性项目如何排布。  
5.行(Line)  
根据 flex-wrap 属性，弹性项目可以排布在单个行或者多个行中。此属性控制侧轴的方向和新行排列的方向。  
6.尺寸(Dimension) 
根据弹性容器的主轴与侧轴，弹性项目的宽和高中，对应主轴的称为主轴尺寸(main size) ，对应侧轴的称为 侧轴尺寸(cross size)。  
min-height 与 min-width 属性初始值将为 0;   
flex 属性是 flex-grow、flex-shrink 和 flex-basis 属性的简写，描述弹性项目的整体的伸缩性。
### 定义一个弹性盒以及圣杯布局
<a href="https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes">地址</a>

	

