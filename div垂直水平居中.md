## 在长宽固定的情况下，div垂直水平居中的几种方法 ：

### 第一种：采用绝对定位，并且用百分比计算，比较常用

<style> /*方法1：*/	.left{	width: 200px;	height: 300px;	background-color:blue;	position: absolute;	left: 50%;	top:50%; margin-left: -100px;	margin-top: -150px;	} </style> <div class="main"> <div class="left"></div> </div>

### 第二种：同样是绝对定位，把上下左右都置为0

<style> /*方法2：*/ .left{	width: 200px;	height: 300px;	background-color:blue;	margin:auto;	position:absolute;	left: 0; right: 0;	top: 0;	bottom: 0; } </style> <div class="main"> <div class="left"></div> </div>

### 第三种：flex布局，需考虑兼容性

<style>	html,body{margin: 0;height: 100%} .main{ display: flex; justify-content: center; align-items: center; height: 100%; } .left{	width: 200px;	height: 300px;	background-color:blue;	} </style> <div class="main"> <div class="left"></div> </div>
## 提示：以上均为特定情况下的特定布局，在实际应用中，具体情况还要具体分析