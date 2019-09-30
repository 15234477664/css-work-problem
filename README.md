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
超出部分变为.....
```css
overflow: hidden;
text-overflow:ellipsis;
white-space: nowrap;
```
多行以后变成......
```css
display: -webkit-box;  
-webkit-box-orient: vertical;
-webkit-line-clamp: 2;
overflow: hidden;
```
竖排文字居中
```css
writing-mode:vertical-lr;
text-align: center;
```
