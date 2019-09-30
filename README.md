# css-work-problem（css工作中遇到的问题总结）
## 消除苹果按钮样式
```css
-webkit-appearance: none;
```
## textarea不能拖拽
```css
resize: none
```
## 规定段落中的文本不进行换行
```css
white-space: nowrap 
```
## 换行
```css
white-space: pre-line
```
## 自动换行
```css
word-wrap: break-word
```
## 将段落的第一行缩进 xxx像素
```css
text-indent:填写要缩进的px
```
## 字间距
```css
letter-spacing:3px;   
```
## input框获取焦点时失去焦点边框
```css
resize: none
```
## 超出部分变为.....
```css
overflow: hidden;
text-overflow:ellipsis;
white-space: nowrap;
```
## 多行以后变成......
```css
display: -webkit-box;  
-webkit-box-orient: vertical;
-webkit-line-clamp: 2;
overflow: hidden;
```
## 竖排文字居中
```css
writing-mode:vertical-lr;
text-align: center;
```
## 旋转180度
```css
transform: rotate(180deg);  
```
## 修改input单选框样式：
```css
.elect_btn_img{
    width:0.52rem;
    height:0.52rem;
    position: absolute;
    background:url("../images/cart/check1.png");
    background-size:0.52rem 0.52rem;
    border-radius:50%;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0;
    margin: auto;
    outline: none;
    -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
    -webkit-appearance: none;
    border: 0;
}
.elect_btn_img:checked {
    background:url("../images/cart/check2.png");
    background-size:0.52rem 0.52rem;
}
```
## 修改selet
```css
select{
    padding: 0 10px;
    appearance:none;
    -moz-appearance:none;
    -webkit-appearance:none;
    /*在选择框的最右侧中间显示小箭头图片*/
    background: url(../images/arrow.png)no-repeat scroll right center transparent;
    background-size:20px auto;
    /*为下拉小箭头留出一点位置，避免被文字覆盖*/
}
```
## 在标题两边加边线
```css
.box_sub-title:before, .box_sub-title:after {
    display: inline-block;
    content: '';
    border-top: 1px solid #484848;
    width:50px;
    margin: 10px 30px;
}
```
## 实星五角星：&starf;
## 空星五角星：&star;
## a标签去除点击的蓝色
```css
-webkit-tap-highlight-color:transparent;
```
## CSS水平垂直居中常见方法总结：
1.定位布局
```html
<div class="box">
    <div class="content">
    </div>
</div>
```
```css
.box {
    background-color: #FF8C00;
    width: 300px;
    height: 300px;  position: relative;}
.content {
    background-color: #F00;
    width: 100px;
    height: 100px;
    position: absolute;
    left: 50%;
    top: 50%;
    margin: -50px 0 0 -50px;
}
```
2.flex布局：
```html
<div class="box">
    <div class="content">
    </div>
</div>
```
```css
.box {
    background-color: #FF8C00;
    width: 300px;
    height: 300px;
    display: flex;//flex布局
    justify-content: center;//使子项目水平居中align-items: center;//使子项目垂直居中}
.content {
    background-color: #F00;
    width: 100px;
    height: 100px;
}
```
3.table-cell布局：
因为table-cell相当与表格的td，td为行内元素，无法设置宽和高，所以嵌套一层，嵌套一层必须设置display: inline-block;td的背景覆盖了橘黄色，不推荐使用
```html
<div class="box">
    <div class="content">
        <div class="inner">
        </div>
    </div>
</div>
```
```css
.box {
    background-color: #FF8C00;//橘黄色
    width: 300px;
    height: 300px;
    display: table;
}
.content {
    background-color: #F00;//红色
    display: table-cell;
    vertical-align: middle;//使子元素垂直居中
    text-align: center;//使子元素水平居中
}
.inner {
    background-color: #000;//黑色
    display: inline-block;
    width: 20%;
    height: 20%;
}
```
## 禁止复制功能：
```css
* {
     -webkit-touch-callout:none;
     -webkit-user-select:none;
     -khtml-user-select:none;
     -moz-user-select:none;
     -ms-user-select:none;
     user-select:none;
 }
 /*设置IOS页面长按不可复制粘贴，但是IOS上出现input、textarea不能输入，因此将使用-webkit-user-select:auto;*/
input,textarea {
    -webkit-user-select:auto; /*webkit浏览器*/
    margin: 0px;
    padding: 0px;
    outline: none;}
 ```
