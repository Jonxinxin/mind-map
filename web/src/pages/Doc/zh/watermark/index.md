# Watermark实例

> 0.2.24+

`Watermark`实例负责显示水印，可通过`mindMap.watermark`获取到该实例。

## 方法

### draw()

重新绘制水印。

注意：非精确绘制，会绘制一些超出可视区域的水印，如果对性能有极致要求，推荐自行开发水印功能。

### updateWatermark(config)

更新水印配置。示例：

```js
mindMap.watermark.updateWatermark({
    text: '水印文字',
    lineSpacing: 100,
    textSpacing: 100,
    angle: 50,
    textStyle: {
      color: '#000',
      opacity: 1,
      fontSize: 20
    }
})
```