# StarrySky

- 作者: DoWake
- 描述：使用 Canvas 绘制星空
- 日期：2023/03/02

# 演示地址

[StarrySky](http://starrysky.mengxing.cc)

#使用教程

## 引入 JS

`<script src="StarrySky.js"></script>`

## 初始化

`StarrySky.init(document.getElementById("bg"));`

> 传入的参数必须是 Canvas 对象

## 设置星星数量等级

`StarrySky.setStarCountLevel(0.2);`

> 提示：星星过多会导致页面卡顿，浏览器占用大量内存、GPU 资源

## 设置星星速度等级

`StarrySky.setStarSpeedLevel(0.0005);`

## 设置星星颜色

`StarrySky.setStarColorList(["255, 255, 255"], true);`

> 第一个参数若传入数组，则替换全部颜色为传入数组的颜色；若传入单个颜色字符串，则添加此颜色到 color 数组中。
> 第二个参数表示是否立刻替换颜色，true 表示立刻替换，此时已渲染的星星颜色会更改为此时 color 数组中的颜色；false 表示已渲染的星星颜色不改变，新渲染的星星颜色为此时 color 数组中的颜色

## 开始渲染

`StarrySky.render();`

## 销毁

`StarrySky.destroy();`

> 不使用时调用此方法及时释放 GPU 资源
