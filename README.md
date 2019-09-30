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
