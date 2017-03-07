# summary-of-JavaScript-jQuery
some notes for study

HTML: 编写网页内容的语言
CSS：编写网页样式的语言
JavaScript：编写网页交互行为的语言
交互：3步: IPO
1. 输入数据/触发事件 2. 处理数据/响应事件 3. 返回结果


1. 什么是js？
2. 如何编写和运行js
3. 如何保存和使用数据
4. 数据的类型

1. 什么是js?
JavaScript：编写网页交互行为的语言
运行在js解释器/引擎中
*解释执行：先读到的先执行，后读到的相同内容会覆盖前边的内容
JavaScript是互联网第一大语言

Netscape: Navigator  LiveScript
     95年：Java "write once run anywhere"
Netscapt:“像极了Java，一定比Java简单”
     LiveScript-->JavaScript
MS:JScript

ECMA:ECMAScript标准——一纸空文
各浏览器厂商，遵照标准*实现*自己的JavaScript语言

W3C：DOM标准：专门操作网页内容的标准

BOM：专门操作浏览器窗口的编程模型——没标准，各厂商自定义。

JavaScript:ECMAScript（定义核心语法）
          +DOM（定义了操作网页内容的语法）
	  +BOM（定义了操作浏览器窗口的方法）

2. 如何编写和运行js
编写:EditPlus
运行：2种方式：1. 使用浏览器自带的js解释引擎
               2. Node.js——了解
第一个js程序：about:blank-->F12-->console控制台
语法：1. 所有字符串都要用引号包裹
      2. *js区分大小写！*
比如：console.log("Hello world!");
    IE11：console.dir("xxx");
    调用"控制台"的"日志功能"，在控制台中输出一行日志
      document.write("Hello world");
    调用"当前网页"的"输出功能"，在网页中输出一行文字
      write功能：其实向网页中写出一行html内容

如何在网页中编写js程序：3种方式：参照CSS
1. 元素事件中
    事件：元素对鼠标或键盘操作的响
          语法：特殊的属性：on事件名=“js语句”
                比如：单击: onclick="window.alert('')";
		<!--当单击时：-->
		<!--调用浏览器窗口的alert功能，弹出警告提示
    强调：事件中的js语句，只有事件触发时才执行
	document.write();2种情况：
	1. 随网页加载过程输出，写在什么位置就在什么位置输出
        2. 如果网页加载完成后，再调用write，
             会重新启动网页输出流，从第一行开始替换原内容

2. <script>元素中:
   <script>元素：网页内专门保存一组脚本块的元素
   
3. 外部.js文件中：2步：1. 新建.js文件；
	2. 引入外部.js文件：<script src="xxx.js"></script>
   强调：<script>要么用于保存内部脚本块
                 要么用于引入外部脚本文件
         不能同时使用src属性和内部脚本块。
	 如果同时使用，仅src生效


js调试：*只要效果出不来，就开控制台*
    错误：1. 同一<script>内,出错位置之前的代码，正常执行
                                ...之后的代码，不执行
          2. 不同<script>之间的错误，不会相互影响！
    debug：控制台中,会显示：
          1. 错误类型:错误原因            出错位置的链接












