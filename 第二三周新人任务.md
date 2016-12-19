# week2-3
### 第二周task2  
![](http://img1.ph.126.net/sI-WnTqxzRSqSS3B9KzOpA==/6630162867629341750.jpg)

在这个表单中我用到的一些重要元素：
> * **input**元素: 根据不同的type属性有text（定义用于文本输入的单行输入字段）、radio（单选按钮允许用户在有限数量的选项中选择其中之一）、submit（定义用于向表单处理程序（form-handler）提交表单的按钮）、checkbox  
> * **label**元素：在 label 元素内点击文本，就会触发此控件。当用户选择该标签时，浏览器就会自动将焦点转到和标签相关的表单控件上。"for" 属性可把 label 绑定到另外一个元素。 "for" 属性的值设置为相关元素的 id 属性值  
> * **textarea**元素：多行文本框
> * **select**元素：创建单选或多选菜单，选项是`option`

### 第二周task3
![](http://img0.ph.126.net/MzW1HjFESthzEGUPvNYdGw==/6630646652745740427.jpg)

> * 虚线：`<hr border-style="dashed">`
> * 链接：**:hover** 选择器用于选择鼠标指针浮动在上面的元素，可用于所有元素，不只是链接。:link 选择器设置指向未被访问页面的链接的样式，:visited 选择器用于设置指向已被访问的页面的链接，:active 选择器用于活动链接。
> * **counter-reset**元素:设置某个选择器出现次数的计数器的值（？懵）
> * counter-increment:对部分和子部分进行编号（比如 "Section 1"、"1.1"、"1.2"）的方法：
```
h1 {counter-reset:subsection;}
h1:before
{
counter-increment:section;
content:"Section " counter(section) ". ";
}`
```
> * **:before**伪元素:在元素之前添加内容

### 第三周task1
![](http://img1.ph.126.net/soyzFpndJUnkQxxeQe2Jbw==/6619171049887032715.png) 

浮动会产生副作用：背景不能显示、边框不能撑开、margin padding设置值不能显示 
css清除浮动float的方法：
* clear：both 清除上级元素的浮动，会多加html和CSS代码
* 在浮动元素的父元素加上一个clearfix class
* overflow方法，可以很少CSS代码即解决
* inline-block
* `:after`
* line-height: 文本垂直居中

### 第三周task2
![](http://img1.ph.126.net/z-60ofy3POxViRAS4kqMHA==/6619434932677697545.png)

> * `text-overflow: ellipsis` 超出时显示...
> * `white-space: nowrap`强制单行显示所有文本
> * 'overflow: hidden'溢出元素框时内容被修剪不会被显示（三行缺一不可）

###第三周task3
![](http://7xrp04.com1.z0.glb.clouddn.com/task_1_4_1.png)

> * border-radius圆角的四个值按顺序取值分别为：左上、右上、右下、左下。圆角的取值为50%或为宽和高一样的值。
> * position慎用absolute，它会脱离正常文本流
