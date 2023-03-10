# 初生点(施工中)

| 修改日期           | 修改人 | 修改内容 | 所属编辑器版本 |
| ------------------ | ------ | -------- | -------------- |
| 2022 年 9 月 28 日 | 廖悦吾 | 文档创建 | 015            |
|                    |        |          |                |

<strong>阅读本文预计 10 分钟</strong>

本文概述了初生点的工作机制，展示在编辑器创建并使用初生点的过程和初生点在游戏中的应用。教程内容包含初生点功能对象的属性面板，类对象属性和接口以及一个示例工程。

# 什么是初生点

初生点是一个提供游戏运行后玩家角色初次生成位置和朝向的一个对象。进入游戏玩家角色会刷新在初生点位置并面向初生点的正方向。一般游戏中使用初生点来控制玩家初次刷新的位置，例如出现在第一关的场景起点，或者分布于地图的各处。

初生点在编辑器中以功能对象的形式存在，打开编辑器后在左侧资源栏中的“逻辑资源”中，选取“游戏功能对象”，红框中就是初生点，资源 ID 为 109。

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnPCgToswN1JuKabIZ0rwyRR.png)

# 初生点 都包含什么

初生点没有自己的属性和接口，它只是单纯继承父类 GameObject。关于父类 GameObject 见”游戏对象“文档。

# 如何合理利用 / 使用 初生点

### 在编辑器工作区中直接使用：

1. <strong>将</strong><strong>初生点</strong><strong>拖入场景，修改它的位置和旋转</strong>

每个工程中场景里自带一个初生点，位置是世界原点（0， 0，0），世界正方向旋转是（0，0，0）

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnuDyd2mzpkqhzbLbjR0e91b.png)

初生点 Z 轴位置<strong>不可低于 45</strong>，否则角色会刷新到地板下方，持续下坠。

初生点 Z 轴旋转控制角色刷新后的朝向，视频中的蓝色小箭头为朝向。

X 轴 Y 轴旋转则不可点击修改，已做屏蔽

### 在代码中动态生成

1. 动态 spawn 初生点

```ts
// 普通spawn生成，没有优先加载或预加载资源则无法生成
let playerStart= MWCore.GameObject.spawnGameObject("109") as GamePlay.PlayerStart;

// 异步spawn生成
let playerStart= await MWCore.GameObject.asyncSpawnGameObject("109") as GamePlay.PlayerStart;
```

# 使用 初生点 的注意事项与建议

1. 初生点只支持单端使用（服务端）
2. 支持多个初生点，此时玩家角色随机选择一个进行刷新

# 项目案例

无
