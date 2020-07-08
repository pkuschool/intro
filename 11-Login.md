---

permalink: /11/
title: 首次登录
description: 万事之前，皆需登录
next: "12"
last: "10"
layout: default
categories: ["2"]
---


## 之前有其他的学校 Office 365 账号怎么办？

对于**外校**：请先退出原学校的 O365 账号并登录学校发的账号（请注意二者不通用）。

<!-- 对于**衔接班**：如果已经熟悉 Office 365 教育版的使用，请点击右上方那个“目录”按钮，从目录跳转到第三章 -->

## 登录

请点击页面中间那个大大的“登录”按钮，然后先输入纸条上的邮箱，在点继续后输入纸条上的密码。

<div class="card-panel flex-center accent-text">
    <i style="font-size: 30px;" class="material-icons">info_outline</i>
    <span style="font-size: 18px;">您的用户名可能在名字全拼后面包含数字，请务必不要忽略。这意味着之前已经有同姓名全拼的同学了。</span>
    <!-- <span style="font-size: 13px;" class="hide-on-small-and-down">&nbsp;</span> -->
</div>



输入密码之后，会需要您绑定手机号、通过验证码验证手机号并重新设置密码。原因有三：

- 为了账号的安全
- 账号验证会需要发送验证短信/打验证电话
- 未来需要用此手机号重置密码

<!-- <div class="card-panel red yellow-text flex-center">
    <span style="font-size: 30px">⚠</span>
    <span style="font-size: 18px">如您不绑定手机号，<strong>将无法在忘记密码时自行重置密码！！！！</strong>如不设置则需要联系 SubIT 进行重置。
</span></div> -->

手机号建议填一个常用手机号（学校不会泄露您的手机号信息，也不会无缘无故发送短信）。

如果将来有变更，请查看 [教程文章](https://mp.weixin.qq.com/s/dkEssxnH1e2M8w38x8sB2Q) 自助更改。

而密码，请使用强密码 **（需要同时出现：大写字母、小写字母、数字，且位数大于8位，否则无法通过；请不要使用形如“123456”的弱密码）** ，并 **记住此密码** 方便未来使用。

<div class="card-panel flex-center accent-text">
    <i style="font-size: 30px;" class="material-icons">notifications_active</i>
    <span style="font-size: 18px;">你知道吗？曾经有人因为不知道这点设置了几十次密码还没过</span>
</div>

### 小测试
你可以在下方的输入框中测试你的密码是否符合要求
#### 此功能安全吗
> **我们不会记录你的密码**；此功能完全基于JavaScript实现，这是一个客户端脚本语言，即所有计算都由你的电脑执行。这意味着，此网页一旦在浏览器里加载完毕后，就再没有其他任何数据需要从服务器上读取了，即不会再与服务器连接，当然也不会取得你电脑里任何信息了。如果你想确认一下，可以在此网页加载完毕后，关闭网络连接，一切都将继续工作。  

<script>

    var f=false
    function chkPassword(){
        var value=document.querySelector('#pwd').value;
        var icon_el=document.querySelector('#status');
        var pattern=/(?=^.{8,}$)((?=.*\d+))(?![.\n])(?=.*[A-Z]+)(?=.*[a-z])(?=.*[`~!@#$%^&*\(\);:'".>,<\/?|\|\\]*).*$/;
        if(value=="123456"&&!f)
        {
            f=true;
            setTimeout(function(){
                alert("你知道吗,123456是最常用的密码之一。大约每139个密码中就有一个是123456")
            },500);
        }
        if(value.search(pattern)!=-1)
        {
            icon_el.style.color="#4caf50";
            icon_el.innerHTML="verified_user";
        }
        else
        {
            icon_el.style.color="#e23037";
            icon_el.innerHTML="warning";
        }
    }

</script>

<div class="align-center"><strong>密码测试：</strong><input id="pwd" class="dk-t" oninput="chkPassword()" type="text" style="padding:0px 5px; width:300px; " placeholder="输入你的密码" /><i id="status" class="material-icons" style="color:#e23037">warning</i></div>

登录成功后请查看下一页。
