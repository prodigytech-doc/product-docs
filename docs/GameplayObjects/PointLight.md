# 点光源

**阅读本文大概需要 10 分钟**

本文概述了点光源的概念，以及他的所有基础属性，以及如何在编辑器中，如何使用点光源对象。

### 什么是点光源？

- 点光源是从一个点向四周散发的光源效果。比方说家中的圆形灯泡，就是我们所说的点光源。

### 如何编辑点光源？

在【本地资源库】-【游戏功能对象】列表中找到【点光源】，将其拖入到场景中，即完成了点光源的创建。

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnBj8k8cFAFy2KsR7PCULqch.png)

然后我们在对象管理器中找到点光源对象，并点击它，就可以在属性面板(默认右下角)中编辑点光源。点光源有若干定制化属性，以下展开介绍：

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnikVLNF1REgFRvwzzfvoxZC.png)

#### 1、强度

- 开发者可通过滑动滚轮调整点光源的光源强度。
- 数值范围：0-160。

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnQaOeiovbqmDY8DcPsLDWMe.png)

强度为 0 时候的地面

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcn47hLTc8l40Gb2QQ3UeIQMq.png)

强度为 1 时候的地面

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnBSJSsURTJ1Id5rtHLlu68d.png)

强度为 100 时候的地面

#### 2、光颜色

开发者可选择点光源的颜色。

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnAPfTPekBx0y3REt4TtGAAb.png)

颜色选择

演示效果：

#### 3、衰弱半径

- 点光源的衰弱半径控制着光源的扩散范围，半径越大，光源的范围也就越大。
- 演示效果

#### 4、光源衰弱指数

- 点光源的衰弱指数控制着光源向外扩散的衰弱效果，系数越小，扩散效果越强，系数越大，扩散效果越弱。
- 数值范围：0-16。
- 演示效果：

### 如何使用点光源？

- 点光源是营造气氛和制作恐怖游戏时，很必要的功能之一。这里我们推荐可以通过脚本挂载到角色身上，将周围的环境光源降低。（目前点光源性能消耗较大，不建议使用数量超过 3 个）
