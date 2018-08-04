1.给每个`.panel`绑定click事件，当用户点击某个`.panel`时就会给该`.panel`添加`.open`名称

2.由于`.open`已经设置了样式：

```css
.panel.open {
  flex: 5;
  font-size:40px;
}
```

所以这个`.panel`的`flex`属性值就会由1->5，`font-size`由20px->40px

3.而这个变化过程也触发了`.panel`的`transition`属性：

```css
.panel{
transition:
  font-size 0.7s cubic-bezier(0.61,-0.19, 0.7,-0.11),
  flex 0.7s cubic-bezier(0.61,-0.19, 0.7,-0.11)
}
```

4.当`font-size`和`flex`转换完后会触发`transitionend`事件