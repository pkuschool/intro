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
        var charging=null;
        var chargingTime=null;
        var dischargingTime=null;
        var level=null;
        navigator.getBattery().then(function(battery) {
            charging = battery.charging;
            chargingTime = battery.chargingTime;
            dischargingTime = battery.dischargingTime;
            level = battery.level*100+"%";
            battery.addEventListener('chargingchange', function() {
                charging = battery.charging;
            });
            battery.addEventListener('chargingtimechange', function() {
                chargingTime = battery.chargingTime;
            });
            battery.addEventListener('dischargingtimechange', function() {
                dischargingTime = battery.dischargingTime;
            });
            battery.addEventListener('levelchange', function() {
                level = battery.level*100+"%";
            });
        });
        setInterval(function(){
            document.querySelector('#charging').innerHTML=charging;
            document.querySelector('#chargingTime').innerinnerHTMLText=chargingTime;
            document.querySelector('#dischargingTime').innerHTML=dischargingTime;
            document.querySelector('#level').innerHTML=level;
        },200);
        document.querySelector('#javaEnable').innerHTML=navigator.javaEnabled();
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

### 电池属性

<div id="battery">

    <p>是否充电:<code id="charging"></code></p>
    <p>还需充电时间:<code id="chargingTime"></code></p>
    <p>剩余电量:<code id="dischargingTime"></code></p>
    <p>剩余百分比:<code id="level"></code></p>

</div>

### 多点触控

<p>最大触控点: <code id="touchpoint"></code></p>

### JAVA

<p>是否启用JAVA: <code id="javaEnable"></code></p>
