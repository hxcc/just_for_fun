# GxlCMS v1.1.4存在储存xss漏洞

漏洞POC

`123"123>undefined<script>alert(12)</script>`

漏洞位置

​       在`添加小说数据界面`可以输入POC导致XSS触发

http://127.0.0.1/gxl/index.php?s=Admin-Index

![1551775513460](C:\Users\jxy\AppData\Roaming\Typora\typora-user-images\1551775513460.png)

漏洞分析

![1551775634782](C:\Users\jxy\AppData\Roaming\Typora\typora-user-images\1551775634782.png)

![1551775650262](C:\Users\jxy\AppData\Roaming\Typora\typora-user-images\1551775650262.png)

发现未对代码进行过滤

漏洞证明

![1551775703985](C:\Users\jxy\AppData\Roaming\Typora\typora-user-images\1551775703985.png)

前台后台均可触发XSS







