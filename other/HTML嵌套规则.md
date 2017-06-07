## 元素类型类：
* 块元素：
     address、blockquote、center、dir、div、dl、dt、dd、fieldset、form、h1~h6、hr、isindex、menu、noframes、noscript、ol、p、pre、table、ul等
* 内联元素：
     a、abbr、acronym、b、bdo、big、br、cite、code、dfn、em、font、i、img、input、kbd、label、q、s、samp、select、small、span、strike、strong、sub、sup、textarea、tt、u、var等
 
## 嵌套规则：
* 块能包含块和内联，内联只能包含内联
* 块元素可以包含内联元素或某些块元素，但内联元素却不能包含块元素，它只能包含其它的内联元素
* 标题和段落中不能包含块
* 有几个特殊的块级元素只能包含内嵌元素，不能再包含块级元素，这几个特殊的标签是
> h1、h2、h3、h4、h5、h6、p、dt
* 块与内联不能并列
* 块级元素与块级元素并列、内嵌元素与内嵌元素并列

## 注意：
* li是块级元素，可以嵌套块级元素（包括ul）。
* 有些标签是固定的嵌套规则，比如ul包含li、ol包含li、dl包含dt和dd等等。
* \<textarea>不可以嵌套自己，自行参考该标签在w3School教程上的实例。
* 这里说明一下，虽然可以可以使用display设置block和inline，但以此来定义嵌套关系很显然不严谨。（不知道搜索引擎会不会抓取CSS内容？）

## 进阶知识：
* WEB标准系列HTML元素嵌套
* 由于现在自己接触不到HTML5，所以先保留
* 嵌套错误可能引起的问题
* 元素开始与结束标签嵌套错误，页面可以在大部分浏览器被正常解析，IE9会出现解析错误
* 在\<p>元素内嵌入\<div>等元素造成所有浏览器的解析错误
* 在<h1>\~<h6>元素内嵌入\<div>等元素所有浏览器可以解析正常
* 在\<a>元素内嵌入\<a>元素会导致所有浏览器的解析错误（a也不可嵌套button，input等交互元素）
* 在列表元素\<li>\<dt>\<dd>等插入非列表兄弟元素会导致IE6\IE7的解析错误
