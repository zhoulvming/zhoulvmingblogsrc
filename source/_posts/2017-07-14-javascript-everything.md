---
title: javascript_everything
date: 2017-07-14 06:59:45
tags: javascript
---

我决定为初学者写一篇博客来介绍一些常见编程技巧，这些技巧可以帮助你写出更加规范，容易维护的代码

## 常量
这个问题哦不仅仅是写JavaScript的开发者们会遇到，在所有的开发语言中都要避免。我们来看一个例子：
```
$elem.on('keydown', function(e) {
  if (e.keyCode == 27) {
    //...
  }
});
```
