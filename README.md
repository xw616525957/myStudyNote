<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [前言](#%E5%89%8D%E8%A8%80)
- [markdown基础语法](#markdown%E5%9F%BA%E7%A1%80%E8%AF%AD%E6%B3%95)
  - [强调](#%E5%BC%BA%E8%B0%83)
  - [*斜体*](#%E6%96%9C%E4%BD%93)
  - [换行](#%E6%8D%A2%E8%A1%8C)
  - [引用](#%E5%BC%95%E7%94%A8)
  - [列表](#%E5%88%97%E8%A1%A8)
  - [超链接](#%E8%B6%85%E9%93%BE%E6%8E%A5)
  - [插入图片](#%E6%8F%92%E5%85%A5%E5%9B%BE%E7%89%87)
  - [插入引用标注](#%E6%8F%92%E5%85%A5%E5%BC%95%E7%94%A8%E6%A0%87%E6%B3%A8)
  - [插入文章目录](#%E6%8F%92%E5%85%A5%E6%96%87%E7%AB%A0%E7%9B%AE%E5%BD%95)
  - [水平分区线](#%E6%B0%B4%E5%B9%B3%E5%88%86%E5%8C%BA%E7%BA%BF)
  - [**代码段**](#%E4%BB%A3%E7%A0%81%E6%AE%B5)
- [Markdown高级语法](#markdown%E9%AB%98%E7%BA%A7%E8%AF%AD%E6%B3%95)
  - [流程图](#%E6%B5%81%E7%A8%8B%E5%9B%BE)
  - [时序图](#%E6%97%B6%E5%BA%8F%E5%9B%BE)
- [Markdown相关软件](#markdown%E7%9B%B8%E5%85%B3%E8%BD%AF%E4%BB%B6)
- [结语](#%E7%BB%93%E8%AF%AD)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


 [TOC] 


# 前言  
  
> 一直比较羡慕有些博主博客排版精致，比如文章的索引，引用块和代码块的样式等，当然还有一些开源代码库中readme中排版的样式也特别精致。只知道有Markdown这么个东西，因为太懒从来都没有好好看看Markdown的语法。最近打算整理下自己项目中的Readme说明，就大概看了下MarkDown的语法，粗略的看了一遍后深深的被她吸引，记录下来以供参考。  

# markdown基础语法  
 
## 强调
**着重强调**
```
**着重强调**
```

## *斜体* 
```
*斜体*
```  
## 换行
```
在行尾输入两个或以上的空格，然后回车
```
## 引用
>这句话是引用的，看看，自动加上引用样式了  
这行还是引用
>>这个是嵌套引用
这个还是第二层嵌套  

>>>这个是第三层嵌套  

>继续第一层嵌套  


```
引用只需要在被引用的内容段落开头加上右尖括号('>')即可。你可以选择只在开头加一个。也可以在每行前面都加一个，效果是一样的。
多个>表示嵌套引用（如>>,>>>）
需要一个视觉上的空行表示嵌套的结束
例：
>这句话是引用的，看看，自动加上引用样式了  
这行还是引用
>>这个是嵌套引用
这个还是第二层嵌套  

>>>这个是第三层嵌套  

>继续第一层嵌套  

```
##分级标题  
```
分别表示不同的标题分级
 #,##,###,####,#####,######,#######
也可以用
这是一级标题
======
这是二级标题
------
```  
## 列表
* 列表1
* 列表2
* 列表3
+ 列表1
+ 列表2
- 列表3
1. 列表1
2. 列表2
3. 列表三


```
无序可以用*，+，-作为列表标记，有序列表可以用1. （数字+英文句点+空格）标记
```
## 超链接
[惠租车](https://www.huizuche.com)  
```
[惠租车](https://www.huizuche.com)
```
## 插入图片
![图片链接](http://cdn.qiniu.hzc.huizuche.com/idl/idl-big.png) 
```
![图片链接](http://cdn.qiniu.hzc.huizuche.com/idl/idl-big.png)
```  
## 插入引用标注
Markdown语法[^mark] 
```
引用处：
 [^mark] 
 如：Markdown语法[^mark] 
引用说明处：
如：
[^mark]:这是一个引用标注[维基百科Markdown](https://zh.wikipedia.org/wiki/Markdown)
```  
  
## 插入文章目录  
```
文章任何需要插入目录的地方
[TOC]
```
## 水平分区线  
***
```
以下每一种写法都产生一条水平分区线
* * *
***
*****
- - -
---------------------------------------
```

## **代码段**
``` javascript
function GetData(){
	$.ajax(url).success(function(data){
		console.log(data);
	}).error(function(s,s,d){
		console.log(d);
	})
}
```
` ```javascript
function GetData(){
	$.ajax(url).success(function(data){
		console.log(data);
	}).error(function(s,s,d){
		console.log(d);
	})
}```
`
# Markdown高级语法
##表格
|Item       |标题1     |标题二    |
|:----------|--------:|:-------:|
|左对齐      |    右对齐|   中间对齐|
|左         |        右|        中|  

```
|Item       |标题1     |标题二    |
|:----------|--------:|:-------:|
|左对齐      |    右对齐|   中间对齐|
|左         |        右|        中|
```  

##数学公式[^math]  
$$\alpha  
　A　\beta　B　\gamma　\Gamma　\delta　\Delta　\epsilon　E \varepsilon　　\zeta　Z　\eta　H　\theta　\Theta　\vartheta \iota　I　\kappa　K　\lambda　\Lambda　\mu　M　\nu　N \xi　\Xi　o　O　\pi　\Pi　\varpi　　\rho　P \varrho　　\sigma　\Sigma　\varsigma　　\tau　T　\upsilon　\Upsilon \phi　\Phi　\varphi　　\chi　X　\psi　\Psi　\omega　\Omega$$
**行内公式**:$\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$
**块级公式**：$$	x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a} $$
```
  公式中常见的字母
$$\alpha  
　A　\beta　B　\gamma　\Gamma　\delta　\Delta　\epsilon　E \varepsilon　　\zeta　Z　\eta　H　\theta　\Theta　\vartheta \iota　I　\kappa　K　\lambda　\Lambda　\mu　M　\nu　N \xi　\Xi　o　O　\pi　\Pi　\varpi　　\rho　P \varrho　　\sigma　\Sigma　\varsigma　　\tau　T　\upsilon　\Upsilon \phi　\Phi　\varphi　　\chi　X　\psi　\Psi　\omega　\Omega$$
**行内公式**:$\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$
**块级公式**：$$	x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a} $$
```
## 流程图  
```flow
st=>start: 开始  
e=>end: 结束    
op=>operation: 操作 
cond=>condition: 是否满足条件? 

st->op->cond
cond(yes)->e
cond(no))->op
```  
```
st=>start: 开始  
e=>end: 结束    
op=>operation: 操作   
cond=>condition: 是否满足条件?  

st->op->cond
cond(yes)->e
cond(no))->op
```
## 时序图
```sequence
Client->Server: request
Note right of Server: 服务端响应
Server-->Client: response  
```
```
```sequence
Client->Server: request
Note right of Server: 服务端响应
Server-->Client: response
```占位符
```

# Markdown相关软件
>专为印象笔记（Evernote）打造的Markdown编辑器https://maxiang.io/  
>作为在线的Markdown编辑器，简书不错http://www.jianshu.com/  


# 结语 
>以上都是我看完语法后，自己一个个敲出来的，就当是以后的备用手册了，后面一边使用一边再完善吧。 

[^mark]:这是一个引用标注[维基百科Markdown](https://zh.wikipedia.org/wiki/Markdown)   

[^math]:数学公式参照http://oiltang.com/2014/05/04/markdown-and-mathjax/
