---

permalink: /about-project
title: 关于此项目
description: 对这个项目的介绍
next: ./index.html
last: "none"
ifshow: -1
layout: default
---

# 新生指南

北大附中的新生指南。

让新生快速了解学校的基础架构、必知信息、相关平台的使用等信息。

## 目录

- 第一章 欢迎 （欢迎一下，介绍一些基本概念，框架已经搭好了；号码首位为0）
- 第二章 O365 （SubIT 会写的基础使用手把手教程，欢迎提出意见；号码首位为1）
- ~~第三章 大家说 （学长学姐们想对新生说什么？书院想一步到位直接晒出二维码？号码首位为2）~~
- 第三章 后续安排


## 加入编辑

首先你需要（注册）一个 GitHub 账号，然后访问 [https://github.com/orgs/pkuschool/sso](https://github.com/orgs/pkuschool/sso) 进入 pkuschool 组织，最后回到此库。

凡是在此组织内的人，均可编辑。

需要编辑什么文档，直接网页版进入文件编辑即可。


### 编辑指南

要编辑，点击任何一篇的右上角的铅笔按钮即可开始编辑，在[仓库首页](https://github.com/pkuschool/intro)点击 ```Create New File``` 即可新建

新增文件时，文件名应为：

序号-概要英文单词.md（如 ``` 01-Welcome.md ```）

并且，请注意 YAML Front Matter（比如，这篇readme的顶上就有一个），示例是*（注意上下的三个“-”和英文冒号后面的空格不能忽略）*：

```
---

permalink: /[号码，一般为数字，意味着访问时此页面实际的链接，后面必须加斜杠（英文！）]/
title: [标题]
description: [一句话简介，可不写]
next: ../[下一篇文章的号码]/
last: ../[上一篇文章的号码]/
author:
    - [作者列表，署上你自己的名字，美滋滋]
    - [假装有另一位作者]
layout: default

---
```

编辑时，请在上方的 author 里面加上自己的名字，格式见上方。

改文件就像记事本一样简单，简单介绍下 Markdown 最基础的格式：

```markdown

## 我是二号标题！其他的，请类推。

段落之间要有空格，
不然不会换行

- 我是列表

**我是粗体** *我是斜体*

[我是链接显示文字，右边那个是链接指向](#)
```

您也可以上网查找相关资料。

图片引用形式：按这里的特点，应该是：

```
![图片描述](../img/[你强行传到img文件夹的图片文件名])

当然有图床的话，可以直接：

![图片描述（建议填写）](图片链接)
```

上传在[仓库首页](https://github.com/pkuschool/intro)点击 Upload File，拖进去就行

---

编辑完之后，不要忘记点下方的 Commit Changes 保存更改哦！

PS: 更新很快，请尽快写完。

## 想改页面的外观？

请围观```_layouts/default.html```，需要有一定的HTML/CSS/Materialize/Jekyll基础。

## 什么，还不懂？

请联系<liuyuchen1@i.pkuschool.edu.cn>
