---
title: Markdown语法入门看这篇就够了
urlname: Markdown语法入门看这篇就够了
date: 2018-05-06 12:10:55
categories: 
	- 技能
	- Markdown
tags: 
	- 工具书
---

## 标准Markdown语法

### 段落 

	这个文档本身就是使用Markdown编写的。
	Markdown编辑器允许你通过编写易读、易写的富文本格式，然后很方便就可以转换成有效的HTML。

### 标题
Setxt-style:
```
标题1
===
标题2
---
```
atx-style（尾部的 `#` 是可选的）：
```
# 标题1 #
## 标题2 #
###### 标题6 #
```
### 强调或突出
```
*突出*	**强调**
_突出_	__强调__
```
### 链接
内联风格（`title` 是可选的）：
```
[百度官网](http://www.baidu.com "Title")
```
引用风格（`title` 是可选的）：
```
[百度官网][id]。之后，可以在文章的任意地方，定义这个链接:
[id]:http://www.baidu.com "Title"
```
Email
```
作者的email链接
```
### 图片
内联风格（`title` 是可选的）：
```
![alt text](http://wx4.sinaimg.cn/mw690/0060lm7Tly1fqchde4zoaj309v08cglq.jpg "Title")
```
引用风格（`title`是可选的）：
```
![alt text][id]
[id]: http://wx4.sinaimg.cn/mw690/0060lm7Tly1fqchde4zoaj309v08cglq.jpg "Title")
```
### 列表
有序列表：
```
1. 列表项 1
2. 列表项 2
```
无序列表：
```
* 列表项 1
* 列表项 2

- 列表项 3
- 列表项 4
```
列表项缩进两个空格就可以创建一个嵌套的列表：
```
1. 列表项 1
 1. 嵌套的列表可以是有序的
 2. 格式和正常的有序、无序列表没有差异
2. 列表项 2
 * 嵌套的列表可以是无序的
 	* 这个嵌套的列表项有有四个空格的缩进，因为它的父列表项自身就带有2个空格的缩进
  * 还允许更多层的嵌套
3. 列表项 3
```
### 引用
```
>段落前面添加大于号和空格，就能够形成引用段落。
>> 这是嵌套的引用。
```
### 内联代码

`内联代码`使用反映好包含
你也可以像`` `这样` ``转义反引号
### 代码块
每行缩进4个空格或者1个tab：
```
这是正常的段落。记得在使用tab的时候，在上面空一行。
这是代码块。
```
### 水平分割线
三个或更多的星号或下划线：
```
___
* * *
*****
_ _ _ _ _ _ 
```
### 强制换行
在行尾输入两个空格或者`<br/>`：
```
我在上一行
我在下一行
```
## GitHub Flavored Markdown语法
_ _ _
### 链接自动展示

http://www.baidu.com
### 删除线
通过两个波浪号将字符包含：

~~删除的文本或已完成的待办事项~~
### 围栏式代码块

```
标准的Markdown通过每行开头的四个空格将文本转化成代码块，而GFM支持围栏式代码块。只要将代码用```包含起来即可，不需要四个空格的缩进。
```
### 表格
这是个简单的表格：
```
First Header | Second Header | Third Header
------------ | :------------: | ---------:
Content Cell | Content Cell | Content Cell
Content Cell | Content Cell | Content Cell
```
出于完美考虑，可以把两端都包围起来：
```
| First Header | Second Header | Third Header |
| ------------ | :------------: | ---------: |
| Content Cell | Content Cell | Content Cell |
| Content Cell | Content Cell | Content Cell |
```