---

title: 第二章·希悦校园
description: 一个你又爱又恨的系统，尤其喜欢咕咕咕🕊
permalink: /30/
next: "31"
last: "06"
layout: default
author:
    - 何天阳
    - 张子健
categories: ["1"]

---
<script>
  function IsPC() {
    const userAgentInfo = navigator.userAgent;
    const Agents = ["Android", "iPhone",
          "SymbianOS", "Windows Phone",
          "iPad", "iPod"
        ];
    let flag = true;
    for (let v = 0; v < Agents.length; v++) {
      if (userAgentInfo.indexOf(Agents[v]) > 0) {
        flag = false;
        break;
      }
    }
    return flag;
  }
  document.addEventListener('DOMContentLoaded', function () {
    const elems = document.querySelectorAll('img');
    const instances = M.Materialbox.init(elems);
    if (!IsPC()) {
      document.querySelector('#mobile-hint').removeAttribute('hidden');
    }
  });
</script>

在北大附中，我们使用一个叫做“希悦”的系统来将进行诸如课程管理、作业提交等事务 那么，什么是希悦？

<div class="card-panel flex-center accent-text">
  <i style="font-size: 30px;" class="material-icons">info_outline</i>
  <span style="font-size: 18px;">你将会在选完书院之后获得自己的希悦账户（因为学号和书院有关）</span>
</div>

## **总览**

下面的这个网址是希悦的**登录网址**，很重要，请你**务必记住**！
<div class="card-panel flex-center accent-text">
  <i style="font-size: 30px;" class="material-icons">query_builder</i>
  <span style="font-size: 22px;">
    <a href="https://bdfz.seiue.com" target="_blank">bdfz.seiue.com</a>
  </span>
</div>
<br />
**登录之后，你将看到这样的一个页面**

![希悦首页](https://z3.ax1x.com/2021/05/19/g5wiJH.png)
<div class="card-panel flex-center accent-text" id="mobile-hint" hidden>
  <i style="font-size: 30px;" class="material-icons">error_outlined</i>
  <span style="font-size: 18px;">
    如果你发现你的设备打开希悦之后不太对劲<br /><br />
    那么看一看你是不是用的<strong>手机端或者窄屏设备</strong>。<br /><br />
    希悦对这样的设备暂时还没有支持，请使用APP【<a href="/32">点我查看教程</a>】
  </span>
</div>


在页面左侧是一个导航栏，上面有些你在北大附中的高中生活中会非常常用。<br>
<br>
> **首页**，点进去也就是你现在看到的这个页面。这是对希悦功能的一个总览。<br>
> **我的档案**，这这里面有能让你心脏骤停的成绩总览。<br>
> **学期课程，活动课程，第一学段课程，第二学段课程**，这里是你的课程们，有关课程的内容你已经在第一章里了解了 <br>
> **导师**，这也是北大附中特有的~~奇怪的~~的制度之一<br>
> **应用中心**，在这里，你可以预约场馆，创建活动，请假<br>

<br>
页面的下半部分是**课表**，你可以在这里查看你的课表。

![课表](https://z3.ax1x.com/2021/05/19/g5wPFe.png)
<br>
