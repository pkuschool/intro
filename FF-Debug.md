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
        document.querySelector('#platform').innerHTML=navigator.platform;
        var languages=navigator.languages;
        for(var i=0;i<languages.length;i++)
        {
            var newlang=document.createElement("li");
            newlang.innerHTML="第"+(i+1)+"语言: "+languages[i];
            document.querySelector('#lang').appendChild(newlang);
        }
        document.querySelector('#memory').innerHTML=navigator.deviceMemory+"GB";
        document.querySelector('#touchpoint').innerHTML=navigator.maxTouchPoints;
    }); 
</script>

### 浏览器内核信息
<code id="corn"></code>

### 当前时间
<code id="time"></code>

### 平台
<code id="platform"></code>

### 语言
<ul id="lang">
</ul>

### 内存
<code id="memory"></code>

### 多点触控
<p>最大触控点: <code id="touchpoint"></code></p>