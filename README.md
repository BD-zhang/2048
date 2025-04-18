## my 2048 application

> use simple javascript and html and alse css to build an easy application without any framework.
> just for fun


### 动画逻辑

🚀 
第 1 步：确定单个格子动画（已经完成）
第 2 步：多个格子动画（滑动时多个格子一起动）
第 3 步：动态计算位置（根据坐标计算动画偏移）
第 4 步：合并动画（合并时轻微放大再缩小）
第 5 步：整合到 2048 游戏逻辑里（每次移动都触发动画）

#### 1.单个格子动画

```css
tile {
 transition: transform .3s ease;
}
```

```js
const tile = document.getElementById('tile')
tile.style.transform = 'translateX(85px)'
```

现在知道了一个格子具体是怎么移动的，当监听到上下左右键移动时，就可以触发格子的移动

#### 2.多个格子动画

