---

permalink: /
title: 欢迎来到北大附中
description: 🎉🎉🎉
last: "none"
next: "02"
author:
    - 刘语辰
    - 张子健
layout: default
topimg: "https://i.loli.net/2021/06/14/zuBUW9QlVeI8RaF.png"
topimg-pos: center center
topimg-author: Yuchen Liu

---
<script>
  document.addEventListener('DOMContentLoaded', function() {
    var elems = document.querySelectorAll('.materialboxed');
    var instances = M.Materialbox.init(elems);
    var elems2 = document.querySelectorAll('.slider');
    var instances2 = M.Slider.init(elems2,{
      // height: (window.innerHeight*0.3 + window.innerWidth*0.2)
      height: calculatedGallerySize
    });
  });
  M.toast({
    html: '<span>本网站由学生社团撰写，不代表官方观点。</span><a class="btn-flat toast-action right" style="color: var(--accent); font-weight: bold;" onclick="M.Toast.dismissAll()">知道了</a>',
    displayLength: 150000,
    activationPercent: 2
  });
</script>
<!-- <script>
  document.addEventListener('DOMContentLoaded',function(){
    if (typeof(Storage) !== "undefined")
    {
      var now_step=localStorage.getItem("step");
      if(now_step!=""&&now_step!=null&&now_step!=undefined)
      {
        M.toast({
            html: '<div style="text-align: left;"><span>是否返回上次阅读进度&nbsp;？</span><br/><a class="btn-flat toast-action left" onclick="M.Toast.dismissAll()">关闭</a><a class="btn-flat toast-action left" onclick="window.location="./intro'+now_step+'">返回阅读进度</a></div>',
            displayLength: 150000,
            activationPercent: 2
        });
        localStorage.setItem("step",'');
      }
    }
  });
</script> -->

<script>
  function IsPC() {
   const userAgentInfo = navigator.userAgent;
   const Agents = ["Android", "iPhone",
         "SymbianOS", "Windows Phone",
         "iPad", "iPod"];
   let flag = true;
   for (let v = 0; v < Agents.length; v++) {
      if (userAgentInfo.indexOf(Agents[v]) > 0) {
         flag = false;
         break;
      }
   }
   return flag;
}

 document.addEventListener('DOMContentLoaded',function(){
   if(!IsPC())
   {
     document.querySelector('#mobile-hint').removeAttribute('hidden');
   }
 });
</script>

<!-- <img src="http://bdfz-cas.pkuschool.edu.cn/assets/login-1a72e4feef0ed4ad47183208b8d0a0aa.png" width="200"> -->

<p style="font-family: '思源宋体 SC', serif; font-size: 22px; ">

<span style="font-size: 25px; font-weight: bold">北大附中致力于培养：</span><br>

个性鲜明、充满自信、敢于负责，<br>

具有思想力、领导力、创新力的杰出公民。<br>

他们无论身在何处，都能热忱服务社会，<br>

并在其中表现出对自然的尊重和对他人的关爱。<br>

</p>

这一段校训，会在你接下来三年的高中生活中充分的体现。

我们将在这一个短短的教程中尝试让你明白这里是什么、接下来该做什么，也请认真阅读。

<!-- 本指南总共 10000 字左右，预计将花费你 30分钟 ~ 1小时。 -->
### 这个新生指南怎么看？

<div class="card-panel flex-center accent-text">
    <i style="font-size: 30px;" class="material-icons">error_outline</i>
    <span style="font-size: 18px;">如果你是还未填报志愿的同学，请点击这里，而不是下一页，我们有给你们的特供内容。<br><a href="/01/" normal class="pill-btn z-depth-1 white-text" style="background-color:#26a69a;margin-top: 5px;" title="点我！">我是未填报志愿的小朋友！</a></span>
</div>


### 在继续前，请注意...

如果没有其他指示，看完并理解一页然后前往下一页；如果有，建议自己去做（尤其是三部分）

我们强烈建议使用 PC 端（实际上更建议使用自己的笔记本电脑 / 二合一设备访问），Chrome 内核的浏览器继续查看此导览。


<div id="mobile-hint" class="card-panel flex-center accent-text" hidden>
    <i style="font-size: 30px;" class="material-icons">perm_device_information</i>
    <span style="font-size: 18px;">请尽可能避免使用手机或 iPad 浏览，这样后续步骤将难以进行。</span>
</div>

请尽量不要将内容一带而过，否则您可能丢失部分的步骤。


<p style="font-size: 25px; font-weight: bold;">友情提示：请家长务必不要代劳，成长是一个不断告别的过程，知您不舍，且目送吧……
</p>
<!-- <div class="card-panel flex-center accent-text">
    <i style="font-size: 30px;" class="material-icons">error_outline</i>
    <span style="font-size: 18px;">本站点正在修订中，内容仅供预览。</span>
</div> -->



