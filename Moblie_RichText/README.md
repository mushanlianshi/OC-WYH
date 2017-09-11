# OC-WYH
富文本方案。

### Web 方案
* 优点
> 富文本编辑器实现比较容易;不涉及  HTML 数据解析棘手问题。

* 缺点
> 一个 web 实现所有，毕竟不是原生控件；若是想实现与原生控件无异的交互体验，需要强大的前端知识。

### 原生方案
* 优点
> 可控性比较强，交互体验好。

* 缺点
> 组装 HTML 数据 或 解析 HTML 数据都不易。


### JS 部分语法记录
* window.getSelection() ;
> 返回一个  Selection 对象，表示用户选择的文本范围或插入符号的当前位置。

* document.close()
> 关闭一个由 document.open 方法打开的输出流，并显示选定的数据

* document.open()
> 打开文档流

* document.write()
> 写入 文档流

* document.createElement()
* document.createTextNode()
* document.createAttribute()
> 标签、文本、属性创建

* HTMLElement.setAttribute()
* HTMLElement.getAttribute()
> 属性获取与设置(对于已有的属性进行覆盖，否则先创建在赋值)

* document. getElementsByClassName()
* document.getElementById()
* document.getElementsByName()
* document.getElementsByTagName()
>  标签元素获取

* innerHTML
> 读或写

* bool = document.execCommand(aCommandName, aShowDefaultUI, aValueArgument)
> 当使用 contentEditable时，调用 execCommand() 将影响当前活动的可编辑元素。
  开启或关闭 的 aCommandName有 :bold 、italic 、strikeThrough 、subscript、superscript、underline

* isEnabled = document.queryCommandEnabled(command);
> 查询浏览器是否支持指定的富文本编辑指令

* window.location
> 衔接跳转。

* JavaScript event对象
> 该对象表示当前事件。

* JQuery的ready函数与JS的onload的区别
> window.onload必须等到页面内包括图片的所有元素加载完毕后才能执行。$(document).ready()是DOM结构绘制完毕后就执行，不必等到加载完毕。
> window.onload不能同时编写多个，如果有多个window.onload方法，只会执行一个。$(document).ready()可以同时编写多个，并且都可以得到执行
> window.onload没有简化写法。$(document).ready(function(){})可以简写成$(function(){})

* blur()
> 当元素失去焦点时发生 blur 事件。该方法常与 focus() 方法一起使用。
```
$(selector).blur()
或
$(selector).blur(function)
```

### 参考文献
* [Web 富文本编辑器](https://github.com/nnhubbard/ZSSRichTextEditor)
* [原生富文本编辑器](https://github.com/littleMeaning/SimpleWord)
* [DOM-API中英文](https://developer.mozilla.org/zh-CN/docs/Web/API)
* [JavaScriptCore 使用](http://www.jianshu.com/p/a329cd4a67ee)
* [JS Event对象了解](http://www.itxueyuan.org/view/6340.html)