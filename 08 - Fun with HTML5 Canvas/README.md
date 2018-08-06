# canvas绘图步骤

1.创建绘画环境

```js
const canvas = document.querySelector('#draw');
const ctx = canvas.getContext('2d');
```

2.配置调色盘

- `lineCap`：笔触的形状，有 round | butt | square 圆、平、方三种。
- `lineJoin`：线条相较的方式，有 round | bevel | miter 圆交、斜交、斜接三种。
- `lineWidth`：线条的宽度
- `strokeStyle`：线条描边的颜色
- `fillStyle`：填充的颜色

3.新建一条路径 `ctx.beginPath();`

4.设置绘制的起点 `ctx.moveTo(lastX, lastY);`

5.设置绘制的终点 `ctx.lineTo(e.offsetX, e.offsetY);`

6.将起点和终点连起来 `ctx.stroke();`

在这里如果句尾不加封号的话会报错
