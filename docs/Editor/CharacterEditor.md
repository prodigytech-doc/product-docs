# 角色编辑工具

::: tip **阅读本文大概需要 20 分钟**

为了帮助开发者快速了解并使用角色编辑工具，本文主要包含以下 2 个内容：

1. 角色编辑工具简介
2. 角色编辑工具使用指南

:::

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnbeN6MP1cK0NuVJ8hCPm5ae.png)

## 1. 角色编辑工具简介

### 1.1 角色编辑工具是什么

角色编辑工具为开发者提供可视化的角色形象编辑能力，通过调整工具中体型、发型、服饰、妆容等选项可以对游戏中的角色形象进行个性化定制。

### 1.2 角色编辑工具的应用场景

编辑状态下自定义游戏角色形象 ↓

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnWQIZPOr6h8CPnMKtgbSuHb.png)

运行状态下自定义游戏角色形象 ↓（通过 API）

<video controls src="https://cdn.233xyx.com/athena/online/80d5190d7e3c4f00971c41347a1def7f.mp4"></video>

### 1.3 角色编辑基础规则

**1.3.1 角色风格**

角色编辑工具目前提供的角色风格主要分为：**二次元风格**、**多边形风格**和**写实风格**。

二次元风格 ↓

| 男  | 女 |
| --------- | ------------ |
| ![](https://cdn.233xyx.com/1681727691521_797.png) | ![](https://cdn.233xyx.com/1681727691476_917.png) |

多边形风格 ↓

| 男  | 女 |
| --------- | ------------ |
| ![](https://cdn.233xyx.com/1681727691613_794.png) | ![](https://cdn.233xyx.com/1681727691429_659.png) |

写实风格 ↓

| 男  | 女 |
| --------- | ------------ |
| ![](https://cdn.233xyx.com/1681727691659_808.png) | ![](https://cdn.233xyx.com/1681727691566_381.png) |

**1.3.2 编辑项**

- **捏人类**

  捏人类编辑项，可以通过调整**部位缩放、拉伸**等参数来改变角色形象。
  可以调节的选项有：**头部相关**和**身材相关**。

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcn3MmoZfByYQXhZ1q5kVD5cg.png)

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnxJDQxJ4aF6Mv7ORteSoSf0.png)

- **换装类**

  换装类编辑项，可以通过**替换资源**、**调整颜色和花纹**等参数来改变角色形象。
  可以替换的资源有：**发型相关**和**服饰相关**。

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcn9FrWYdrvyd6H6mJVK0PWMe.png)

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcni27gIFyFUHg4xzkpBIpLfN.png)

## 2. 角色编辑工具使用指南

### 2.1 角色编辑工具入口

**入口1：编辑 Player 角色形象**

点击 Player 对象属性面板中的“编辑玩家形象”。

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnAjWHP2IUNkDBKRAJtNrUub.png)

**入口2：编辑人形对象角色形象**

点击人形对象 v2 中的“编辑人形对象”。

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnWF1MMi7VJQ9pqsb2g7Hnqe.png)

**入口3：编辑本地角色形象**

双击工程内容中的角色形象数据文件，或点击右键菜单中的编辑选项。

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnhGKs8c7tGUJwrkJ9ehB7Gf.png)

**入口4：新建角色形象**

在工具栏的新建中，选择新建角色，或在工程内容中点击创建形象。

![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnmlnEDiZidFdGm2VsaGW9Pg.png)

### 2.2 角色编辑数据的保存与使用

- **保存**

  编辑 PLayer/人形对象/本地角色文件时，显示**保存**选项，点击保存后将编辑数据更新至 PLayer/人形对象/本地角色文件中。

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnY2G7UGjIoBGG7fk8ZIdYwb.png)

- **另存为**

  点击另存为，将角色编辑数据**整体**或**组合**存储在工程内容的角色分类下。

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnQ6m0UDVD87fQmhe69Wkdaf.png)

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnpZoO1Pwn2eMaYTunt3Ysjd.png)

- **角色编辑数据说明**

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnShP5WzT1dJCM5PTQoyLrhZ.png)

  | 数据名称   | 用途                                 |
  | ---------- | ------------------------------------ |
  | 体型与姿态 | 存储基础、面部相关、身材相关编辑数据 |
  | 发型       | 存储前发、后发部分编辑数据           |
  | 上衣       | 存储上衣部分编辑数据                 |
  | 下衣       | 存储下衣部分编辑数据                 |
  | 手套       | 存储手套部分编辑数据                 |
  | 鞋         | 存储鞋袜部分编辑数据                 |
  | 插槽参数   | 存储插槽调整、物品预览相关编辑数据   |

- **角色编辑数据应用**

  - **编辑时应用**

    将角色形象数据文件拖入主视口，将数据文件中存储的角色数据应用至角色。

  - **运行时应用**

    通过 API 将数据文件中存储的数据应用至角色。

      ```ts
      //调用工程内容-角色数据文件资源ID改变人形对象对应数据
      LoadEditorDataByGuid("<del>GUID</del>")
      //将角色形象同步至多端
      SyncDIYDataBegin()
      ```

### 2.3 角色编辑数据的导入与导出

- **导入**

  点击工程内容-角色分类下**导入角色形象数据**按钮，在资源管理器中选择要导入的文件后将数据导入。（可支持批量导入）

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnqTpR1Hi4f7PW8x0RJTfHMc.png)

- **导出**

  在工程内容-角色分类下选中某个角色形象数据文件，点击右键菜单中**导出**按钮，在资源管理器中选择导出路径后将该数据导出。

  ![](https://wstatic-a1.233leyuan.com/productdocs/static/boxcnWbwlwZrtnkNtF0jtJPqT6d.png)