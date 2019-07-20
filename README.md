# Openlayer3.Echart3-Layer

A new way to combine Openlayer3 with Echart3,Opitimize the render performance.

>2017/10/19更新

优化图层移动、缩放性能，优化动画效果。减少重绘开销。

>早期描述

在使用Echart时，发现百度官方给出了Echart结合百度地图的例子，在地图数据展示方面有很好的效果，同时，目前手上正好有基于Openlayers的数据展示需求，于是，就了解了相关资料，准备采用这个技术方案来完成需求。

通过仔细观察发现，百度地图与echart结合采用的是叠加overlay（实际上就是div，是一个用来存放echart图标的容器而已）的方式，通过捕获百度地图的平移、缩放等事件，通知echart重新绘制图表，以达到echart图表和地图坐标吻合的目的。

参照百度地图的做法，笔者实验了Openlayers3与echart3结合，方案可行。同时，针对用户提出的地图缩放和平移时echart图表明显落后于地图移动的问题，做出了相应的改进。

预览地址：https://wongspark.github.io/examples/Ol3.Ec3-Layer/demo/myfly.html
![OpenlayerE3.gif](/img/Openlayers3E3.gif)


