## `<kbd></kbd>`

## data-*

## justify-content

## document.querySelector

## `<audio></audio>`

例：

```html
<audio src="someaudio.wav">
您的浏览器不支持 audio 标签。
</audio>
```

可以在开始标签和结束标签之间放置文本内容，这样老的浏览器就可以显示出不支持该标签的信息。

|属性       |值        |描述                                              |
|----------|----------|--------------------------------------------------|
|autoplay  |autoplay  |如果出现该属性，则音频在就绪后马上播放。              |
|controls  | controls  |  如果出现该属性，则向用户显示控件，比如播放按钮。    |
|loop      |loop       |如果出现该属性，则每当音频结束时重新开始播放。        |
|muted     |muted     |规定视频输出应该被静音。                             |
|preload   |preload   |如果出现该属性，则音频在页面加载时进行加载，并预备播放。如果使用 "autoplay"，则忽略该属性。|
|src       | url       |要播放的音频的 URL。                                |

## classList

```
classList 属性返回元素的类名，作为 DOMTokenList 对象。

该属性用于在元素中添加，移除及切换 CSS 类。

classList 属性是只读的，但你可以使用 add() 和 remove() 方法修改它。
```

例：为 <div> 元素添加 class
```
document.getElementById("myDIV").classList.add("mystyle");
```
