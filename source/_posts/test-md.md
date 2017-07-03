---
title: GitHub中公钥如何生成和验证1
date: 2017-07-01 22:46:02
tags:
category: "技术"
---

键入命令：ssh-keygen -t rsa -C "email@email.com"，"email@email.com"是你github账号，如下图所示：


<img src="/assets/img/1.png" height="400" width="600" style="margin-left:0">


在系统的用户目录（mac系统为cd ~）下会生成两个文件id_rsa和id_rsa.pub，文本编辑器打开id_rsa.pub文件，复制所有内容，
在github.com登录后找到ssh密钥管理页面，添加新公钥，Title随便，内容就是刚才复制的内容，如下图所示：

<img src="/assets/img/1.png" height="400" width="600" style="margin-left:0">

到这里已经成功绑定本地系统的密钥到github上，以后本地仓库即可通过ssh方式来进行各种git命令操作。
如果是mac等linux操作系统，可能会有设置目录权限的问题，如果发现git提交等不成功，可能要设置下目录权限，一般设置777就行。

{% blockquote %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque hendrerit lacus ut purus iaculis feugiat. Sed nec tempor elit, quis aliquam neque. Curabitur sed diam eget dolor fermentum semper at eu lorem.
{% endblockquote %}

{% blockquote @DevDocs https://twitter.com/devdocs/status/356095192085962752 %}
NEW: DevDocs now comes with syntax highlighting. http://devdocs.io
{% endblockquote %}

{% codeblock %}
alert('Hello World!');
{% endcodeblock %}
