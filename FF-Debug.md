---
permalink: /Debug/
title: 有关浏览器信息
description:
last: "none"
next: "none"
layout: default
categories: ["Debug"]
---

<script>
    document.addEventListener('DOMContentLoaded',function(){
        document.querySelector('#corn').innerHTML=navigator.userAgent;
        var timeZone=document.querySelector('#time');
        timeZone.innerHTML=new Date();
        setInterval(function(){
            timeZone.innerHTML=new Date();
        },1000);
        document.querySelector('#platform').innerHTML=navigator.platform
    }); 
</script>

### 浏览器内核信息
<code id="corn"></code>

### 当前时间
<code id="time"></code>

### 平台
<code id="platform"></code>