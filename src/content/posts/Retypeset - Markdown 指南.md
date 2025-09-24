---
title: Retypeset - Markdown 样式指南
published: 2025-09-23T10:04:45.450Z
description: '本文是 Retypeset 主题的 Markdown 样式指南。它不仅涵盖了标题、列表、图片等基础语法，还详细介绍了如何使用提示块、折叠块、画廊、视频嵌入以及 Mermaid 图表等丰富组件，旨在帮助你更清晰、更顺利地编写和美化文章。'
updated: ''
tags:
  - Guides
  - Markdown
draft: false
pin: 0
toc: true
lang: ''
abbrlink: 'retypeset-markdown-style-guides'
---

## 标题

在文本前添加井号 `#` 与空格，即可创建标题。井号数量对应标题等级。

### 语法

```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

### 效果

#### 四级标题
##### 五级标题
###### 六级标题

## 段落

使用空行分隔文本，即可创建段落。

### 语法

```markdown
孔乙己一到店，所有喝酒的人便都看着他笑，有的叫道：“孔乙己，你脸上又添上新伤疤了！”他不回答，对柜里说：“温两碗酒，要一碟茴香豆。”便排出九文大钱。他们又故意的高声嚷道：“你一定又偷了人家的东西了！”孔乙己睁大眼睛说：“你怎么这样凭空污人清白……”“什么清白？我前天亲眼见你偷了何家的书，吊着打。”孔乙己便涨红了脸，额上的青筋条条绽出，争辩道：“窃书不能算偷……窃书！……读书人的事，能算偷么？”接连便是难懂的话，什么“君子固穷”，什么“者乎”之类，引得众人都哄笑起来：店内外充满了快活的空气。

听人家背地里谈论，孔乙己原来也读过书，但终于没有进学，又不会营生；于是愈过愈穷，弄到将要讨饭了。
```

### 效果

孔乙己一到店，所有喝酒的人便都看着他笑，有的叫道：“孔乙己，你脸上又添上新伤疤了！”他不回答，对柜里说：“温两碗酒，要一碟茴香豆。”便排出九文大钱。他们又故意的高声嚷道：“你一定又偷了人家的东西了！”孔乙己睁大眼睛说：“你怎么这样凭空污人清白……”“什么清白？我前天亲眼见你偷了何家的书，吊着打。”孔乙己便涨红了脸，额上的青筋条条绽出，争辩道：“窃书不能算偷……窃书！……读书人的事，能算偷么？”接连便是难懂的话，什么“君子固穷”，什么“者乎”之类，引得众人都哄笑起来：店内外充满了快活的空气。

听人家背地里谈论，孔乙己原来也读过书，但终于没有进学，又不会营生；于是愈过愈穷，弄到将要讨饭了。

## 居中

支持在 Markdown 里写原生 HTML，所以可以直接用 `<div>` 或 `<p>` 标签并设置 `align` 属性。

### 语法

```
<div align="center">
  这句话会居中显示
</div>
```

### 效果

<div align="center">
  这句话会居中显示
</div>

## 图片

使用半角感叹号 `!` 方括号 `[]` 与圆括号 `()`，即 `![alt](src)` 可添加图片。

在 `alt` 前加下划线 `_` 或者留空 `alt` 即可隐藏图注

### 语法

```markdown
![图片描述](./_images/example.jpeg)

![图片描述](https://image.example.com/image-01.webp)

![_图片描述](./_images/example.jpeg)

![_图片描述](https://image.example.com/image-01.webp)
```

### 效果

![by Dongni Hou](./_images/example.webp)

## 标识元素

包括

- `<sup>` 上标
- `<sub>` 下标
- `<abbr>` 缩写
- `<del>` 删除线
- `<u>` 波浪线
- `<kbd>` 键盘输入
- `<mark>` 高亮
- `color` 颜色 
- `<hr>` 分隔线。

### 语法

```
H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

<abbr title="Graphics Interchange Format">GIF</abbr> 是一种位图图像格式。

书籍是人类进步的<del>楼梯</del>阶梯。

优秀的作家总是会仔细检查<u title="拼写">拚写</u>问题。

按下 <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Delete</kbd> 以结束会话。

大多数<mark>蝾螈</mark>昼伏夜出，以昆虫、蠕虫等小生物为食。

<span style="color:red;">红色文字</span>

使用三个连字符 `---` 或 `<hr>` 标签，即可创建如下分隔线。


---
```

### 效果

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

<abbr title="Graphics Interchange Format">GIF</abbr> 是一种位图图像格式。

书籍是人类进步的<del>楼梯</del>阶梯。

优秀的作家总是会仔细检查<u title="拼写">拚写</u>问题。

按下 <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Delete</kbd> 以结束会话。

大多数<mark>蝾螈</mark>昼伏夜出，以昆虫、蠕虫等小生物为食。

<span style="color:red;">红色文字</span>

使用三个连字符 `---` 或 `<hr>` 标签，即可创建如下分隔线。

---

## 块

### 引用多个段落

使用 `>` 符号和空格，即可创建块引用，其中可包含多个段落

#### 语法

```markdown
> 天地不仁，以万物为刍狗。
>
> **提示**：引用块内可使用 _Markdown 语法_。
```

#### 效果

> 天地不仁，以万物为刍狗。
>
> **提示**：引用块内可使用 _Markdown 语法_。

### 标注引用来源

使用 `<cite>` 或 `<footer>` 标签，即可标注引用来源，同时可通过 `[^1]` 或 `[^note]` 格式插入脚注。

#### 语法

```markdown
> 在我的后园，可以看见墙外有两株树，一株是枣树，还有一株也是枣树。
>
> —— <cite>《秋夜》[^1]</cite>

[^1]: 《[秋夜](https://zh.wikisource.org/wiki/%E7%A7%8B%E5%A4%9C_(%E9%AD%AF%E8%BF%85))》是鲁迅散文诗集《野草》中的第一首散文诗，创作于 1924 年。
```

#### 效果

> 在我的后园，可以看见墙外有两株树，一株是枣树，还有一株也是枣树。
>
> —— <cite>《秋夜》[^1]</cite>

[^1]: 《[秋夜](https://zh.wikisource.org/wiki/%E7%A7%8B%E5%A4%9C_(%E9%AD%AF%E8%BF%85))》是鲁迅散文诗集《野草》中的第一首散文诗，创作于 1924 年。

### 提示块

使用 GitHub 语法 `> [!TYPE]` 或三冒号语法 `:::type`，即可创建提示块。支持 `note`、`tip`、`important`、`warning` 和 `caution` 五种类型。

#### 语法

```GITHUB
> [!NOTE]
> 即使快速浏览，也值得用户留意的信息。

> [!TIP]
> 可选信息，可帮助用户更轻松地完成操作。

> [!IMPORTANT]
> 用户成功所需的关键信息。

:::warning
由于存在潜在风险，需要用户立即关注的关键内容。
:::

:::caution
某些操作可能带来的负面后果。
:::

:::note[自定义标题]
这是一个自定义标题的提示块。
:::
```

#### 效果

> [!NOTE]
> 即使快速浏览，也值得用户留意的信息。

> [!TIP]
> 可选信息，可帮助用户更轻松地完成操作。

> [!IMPORTANT]
> 用户成功所需的关键信息。

:::warning
由于存在潜在风险，需要用户立即关注的关键内容。
:::

:::caution
某些操作可能带来的负面后果。
:::

:::note[自定义标题]
这是一个自定义标题的提示块。
:::

### 折叠块

使用三冒号语法 `:::fold[title]`，即可创建折叠部分。点击标题可以展开或收起。

#### 语法

```GITHUB
:::fold[使用提示]
如果需要添加并非所有读者都会感兴趣的内容，可以将其放在折叠部分。
:::
```

#### 效果

:::fold[使用提示]
如果需要添加并非所有读者都会感兴趣的内容，可以将其放在折叠部分。
:::

### 画廊

使用三冒号语法 `:::gallery`，即可创建图片画廊。水平滚动以查看更多图片。

#### 语法

```
:::gallery
![羊驼](https://image.radishzz.cc/image/gallery/sheep-1.jpg)
![转头](https://image.radishzz.cc/image/gallery/sheep-2.jpg)
![对视](https://image.radishzz.cc/image/gallery/sheep-3.jpg)
![小羊驼](https://image.radishzz.cc/image/gallery/sheep-4.jpg)
![可爱捏](https://image.radishzz.cc/image/gallery/sheep-5.jpg)
:::
```

#### 效果

:::gallery
![羊驼](https://image.radishzz.cc/image/gallery/sheep-1.jpg)
![转头](https://image.radishzz.cc/image/gallery/sheep-2.jpg)
![对视](https://image.radishzz.cc/image/gallery/sheep-3.jpg)
![小羊驼](https://image.radishzz.cc/image/gallery/sheep-4.jpg)
![可爱捏](https://image.radishzz.cc/image/gallery/sheep-5.jpg)
:::

### 代码块

使用三个反引号 ````` 包裹代码，即可创建代码块。

在顶部的反引号后标注语言类型，例如 html、javascript、css、markdown 等，即可实现语法高亮。

#### 语法

````html
```html
<!doctype html>
<html lang="zh-CN">
  <head>
    <meta charset="utf-8" />
    <title>HTML5 示例文档</title>
  </head>
  <body>
    <p>测试</p>
  </body>
</html>
```
````

#### 效果

```html
<!doctype html>
<html lang="zh-CN">
  <head>
    <meta charset="utf-8" />
    <title>HTML5 示例文档</title>
  </head>
  <body>
    <p>测试</p>
  </body>
</html>
```

### 视频

使用双冒号语法 `::youtube{id="videoId"}`，即可嵌入视频。

#### 语法

```GITHUB
::youtube{id="9pP0pIgP2kE"}

::bilibili{id="BV1sK4y1Z7KG"}
```

#### 效果

::youtube{id="9pP0pIgP2kE"}

::bilibili{id="BV1sK4y1Z7KG"}

### X 推文

使用双冒号语法 `::tweet{url="tweetUrl"}`，即可嵌入 X 推文卡片。

#### 语法

```
::tweet{url="https://x.com/hachi_08/status/1906456524337123549"}
```

#### 效果

::tweet{url="https://x.com/hachi_08/status/1906456524337123549"}

### Github 仓库

使用双冒号语法 `::github{repo="owner/repo"}`，即可创建 GitHub 仓库卡片。在页面加载时，从 GitHub API 实时获取仓库数据。

#### 语法

```GITHUB
::github{repo="radishzzz/astro-theme-retypeset"}
```

#### 效果

::github{repo="radishzzz/astro-theme-retypeset"}



## 列表

### 有序列表

#### 语法

```
1. 第一项
2. 第二项
3. 第三项
```

#### 效果

1. 第一项
2. 第二项
3. 第三项

### 无序列表

#### 语法

```
- 列表项
- 图表项
- 更多项
```

#### 效果

- 列表项
- 图表项
- 更多项

### 嵌套列表

#### 语法

```
- 水果
  - 苹果
  - 橙子
  - 香蕉
- 蔬菜
  - 青菜
  - 萝卜
```

#### 效果

- 水果
  - 苹果
  - 橙子
  - 香蕉
- 蔬菜
  - 青菜
  - 萝卜

## 表格

使用三个或多个连字符 `---` 分隔标题，并使用管道符 `|` 分隔每列，即可创建表格。

### 语法

```markdown
| 斜体   | 粗体     | 代码   |
| ----- | ------- | ------ |
| _斜体_ | **粗体** | `代码` |
| _斜体_ | **粗体** | `代码` |
```

### 效果

| 斜体   | 粗体     | 代码   |
| ------ | -------- | ------ |
| _斜体_ | **粗体** | `代码` |
| _斜体_ | **粗体** | `代码` |

## Mermaid 图表

使用代码块包裹 Mermaid 语法，并标注语言类型 `mermaid`，即可创建 Mermaid 图表。

### 语法

````
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
````

### 效果

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

