# shopstore

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


# 项目分析
vue-router
前端路由；Key-Value键值对
key:url 地址栏中的路径
value:相应的组件
注意；项目是上中下结构

路由组建：
Home首页路由组件，Search搜索框路由，Login|Register登录|注册路由
非路由组件：
Header，
Footer 首页有 登录|注册页面没有



<!-- flex布局用法 -->
1. flex-direction：决定主轴的方向（即项目的排列方向）。

row（默认值）：主轴为水平方向，起点在左端。
row-reverse：主轴为水平方向，起点在右端。
column：主轴为垂直方向，起点在上沿。
column-reverse：主轴为垂直方向，起点在下沿。
2. flex-wrap：默认情况下，项目都排在一条线（又称"轴线"）上。flex-wrap属性定义，如果一条轴线排不下，如何换行。

nowrap（默认）：不换行。
wrap：换行，第一行在上方。
wrap-reverse：换行，第一行在下方。
3. flex-flow: flex-direction || flex-wrap

4. justify-content: 定义了项目在主轴上的对齐方式（横行对齐方式）。

flex-start （默认值）：左对齐
flex-end：右对齐
center： 居中
space-between：两端对齐，项目之间的间隔都相等。
space-around：每个项目两侧的间隔相等。所以，项目之间的间隔比项目与边框的间隔大一倍。
5. align-items: 属性定义项目在交叉轴上如何对齐（纵向对齐方式）。

flex-start：交叉轴的起点对齐。
flex-end：交叉轴的终点对齐。
center：交叉轴的中点对齐。
baseline: 项目的第一行文字的基线对齐。
stretch（默认值）：如果项目未设置高度或设为auto，将占满整个容器的高度。
6. align-content： 属性定义了多根轴线的对齐方式。如果项目只有一根轴线，该属性不起作用（纵向对齐方式）。

flex-start：与交叉轴的起点对齐。
flex-end：与交叉轴的终点对齐。
center：与交叉轴的中点对齐。
space-between：与交叉轴两端对齐，轴线之间的间隔平均分布。
space-around：每根轴线两侧的间隔都相等。所以，轴线之间的间隔比轴线与边框的间隔大一倍。
stretch（默认值）：轴线占满整个交叉轴。
7. flex-grow：定义项目的放大比例，默认为0，即如果存在剩余空间，也不放大。

8. flex-shrink：定义了项目的缩小比例，默认为1，即如果空间不足，该项目将缩小。

9. flex-basis：定义了在分配多余空间之前，项目占据的主轴空间（main size）。
浏览器根据这个属性，计算主轴是否有多余空间。它的默认值为auto，即项目的本来大小。
它可以设为跟width或height属性一样的值（比如350px），则项目将占据固定空间。

10. flex：是flex-grow, flex-shrink 和 flex-basis的简写，默认值为0 1 auto。后两个属性可选。
该属性有两个快捷值：auto (1 1 auto) 和 none (0 0 auto)。

11. align-self：允许单个项目有与其他项目不一样的对齐方式，可覆盖align-items属性。默认值为auto，表示继承父元素的align-items属性，如果没有父元素，则等同于stretch。
————————————————
版权声明：本文为CSDN博主「爱吃的喵」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/wing_1989/article/details/105479115