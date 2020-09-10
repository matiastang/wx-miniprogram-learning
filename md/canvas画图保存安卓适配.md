# canvas画图保存

## 问题

![iOS上保存图片](./img/iOS.jpeg)
![安卓上保存图片](./img/android.jpeg)

图片是半透明的所有显示出了背景颜色，所以是canvas在两中手机上的背景颜色不同导致的。

## 处理办法

使用canvas之前，设置canvas的初始颜色为统一的白色就可以了。
```js
let ctx = wx.createCanvasContext('canvas')
ctx.fillStyle = "#ffffff"
ctx.fillRect(0, 0, canvasWidth, canvasHeight)
```
初始为白色画布之后再绘制就不会有这个问题了。