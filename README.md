# JavaScript-Study03
JavaScript学习之jQuery  

***********声明该资料来源于w3school以及网络博客整理，仅供学习交流谢谢！*****  

#### jQuery 库 - 特性  
jQuery 是一个 JavaScript 函数库。  
jQuery 库包含以下特性：  
- HTML 元素选取   
- HTML 元素操作  
- CSS 操作   
- HTML 事件函数  
- JavaScript 特效和动画   
- HTML DOM 遍历和修改  
- AJAX  
- Utilities  

#### jQuery 安装  
1.下载 jQuery  
有两个版本的 jQuery 可供下载：  
Production version - 用于实际的网站中，已被精简和压缩。  
Development version - 用于测试和开发（未压缩，是可读的代码）  
这两个版本都可以从 jQuery.com 下载。  
提示：您可以把下载文件放到与页面相同的目录中，这样更方便使用。  

2.替代方案  
如果您不希望下载并存放 jQuery，那么也可以通过 CDN（内容分发网络） 引用它。  
谷歌和微软的服务器都存有 jQuery 。  

Google CDN:  
```
<head>
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.8.0/jquery.min.js">
</script>
</head>
```
Microsoft CDN:  
```
<head>
<script src="http://ajax.aspnetcdn.com/ajax/jQuery/jquery-1.8.0.js">
</script>
</head>
```
#### jQuery 语法实例  
$(this).hide()  
演示 jQuery `hide()` 函数，隐藏当前的 HTML 元素。  
`$("#test").hide()`  
演示 jQuery hide() 函数，隐藏 id="test" 的元素。  
`$("p").hide()`  
演示 jQuery hide() 函数，隐藏所有 `<p>` 元素。  
`$(".test").hide() `  
演示 jQuery hide() 函数，隐藏所有 class="test" 的元素。  
jQuery 语法  
jQuery 语法是为 HTML 元素的选取编制的，可以对元素执行某些操作。  
基础语法是：`$(selector).action()`  
- 美元符号定义 jQuery  
- 选择符（selector）“查询”和“查找” HTML 元素  
- jQuery 的 action() 执行对元素的操作  

##### 文档就绪函数      
您也许已经注意到在我们的实例中的所有 jQuery 函数位于一个 document ready 函数中：  
```
$(document).ready(function(){

--- jQuery functions go here ----

});
```
这是为了防止文档在完全加载（就绪）之前运行 jQuery 代码。 

#### jQuery 选择器
在前面的章节中，我们展示了一些有关如何选取 HTML 元素的实例。
关键点是学习 jQuery 选择器是如何准确地选取您希望应用效果的元素。
jQuery 元素选择器和属性选择器允许您通过标签名、属性名或内容对 HTML 元素进行选择。
选择器允许您对 HTML 元素组或单个元素进行操作。
在 HTML DOM 术语中：
选择器允许您对 DOM 元素组或单个 DOM 节点进行操作。
jQuery 元素选择器
##### jQuery 使用 CSS 选择器来选取 HTML 元素。
`$("p")` 选取 `<p>` 元素。
`$("p.intro")` 选取所有 class="intro" 的 `<p>` 元素。
`$("p#demo")` 选取所有 `id="demo"` 的 `<p>` 元素。
##### jQuery 属性选择器
jQuery 使用 XPath 表达式来选择带有给定属性的元素。
`$("[href]")` 选取所有带有 href 属性的元素。
`$("[href='#']")` 选取所有带有 href 值等于 `"#"` 的元素。
`$("[href!='#']")` 选取所有带有 href 值不等于 `"#"` 的元素。
`$("[href$='.jpg']")` 选取所有 href 值以 `".jpg"` 结尾的元素。
##### jQuery CSS 选择器
jQuery CSS 选择器可用于改变 HTML 元素的 CSS 属性。
下面的例子把所有 p 元素的背景颜色更改为红色：
实例
`$("p").css("background-color","red");`
