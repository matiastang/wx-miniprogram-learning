# scroll-view中的元素居中

## 开启`enable-flex`
```html
<scroll-view enable-flex="true" scroll-y="true">
    <image style="min-height: 100rpx;" src="{{imageDomain}}image/png/allergy-analysis-8.png"></image>  
    <view>
        
    </view>
</scroll-view>
```
`scroll-view`开`enable-flex="true"`后，文字项目能居中，但是图片没有默认高度，所以需要设置`min-height`样式才有效果。

## 内部嵌套一层

```html
<scroll-view enable-flex="true" scroll-y="true"> 
    <view>
        <image src="{{imageDomain}}image/png/allergy-analysis-8.png"></image> 
    </view>
</scroll-view>
```
嵌套层设置`flex`宽度设置为`100%`也可实现相同效果。