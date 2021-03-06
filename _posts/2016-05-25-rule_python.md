﻿---
layout: post
title:  Python编码规范
date: 2016-05-25
tags: Python 编码规范
---


### 介绍

Python编码规范


### 一.命名规范

**1. 变量命名规范**

> * 变量名表述清楚,使用英文词汇;
> * 命名较长时可使用英文缩写，但尽量使用约定俗成的缩写,例如:position缩写为pos、message缩写为msg;
> * 使用下划线命名法,即全小写英文字母,单词之间使用下划线（“_”）分隔;
> * 变量名前不使用任何表示类型的前缀;
> * 类的私有成员变量以一个下划线“_”开头,例如：self._name;
> * 常量所有字母大写,单词之间使用下划线（“_”）分隔，例如：FRAME_RATE;
> * 不要使用形如__xxxx__的系统保留字命名方式.


**2. 函数命名规范**

> * 命名规则与变量相同（即也是全小写的下划线命名法）.

**3．类的命名规范**

> * 类名使用帕斯卡命名法,即单词首字母大写,其余字母小写,不使用下划线连接,例如：class ChatDialog(DialogBase):;
> * 类名不使用任何前缀，例如：class Player():不要写成class CPlayer():.


**4．目录、文件（模块）命名规范**

> * 目录名和模块名全小写,单词之间直接连接,不使用任何分隔符;
> * 模块名要尽量简短,不包含下划线.

### 二.布局规范

**1. 变量与常量**


> * 尽量避免使用全局变量,除非是作为常量使用,所有常量的定义放在单独一个模块consts.py中，便于共享;
> * 同一个类的所有对象共享的变量使用类的变量;
> * 多行变量赋值语句不要做无谓的对齐,只需要在“=”两边各保留一个空格.

**2.	缩进**

> * 必须使用TAB缩进,禁止使用空格缩进;
> * 编辑器中请设置TAB占用四个字符位,不使用空格代替TAB.

**3. 空格**

> * 双目运算符（如：“+”、“*=”、“<=”、“and”等）,两侧各留一个空格,如：a = b + c、 index < 0 or index >= size;
> * 冒号“:”左侧不加空格，如果用在非行尾,则其右侧加一个空格,例如,字典对象中,d = { key: value }
> * 逗号分隔符的左侧不加空格，右侧加一个空格;
> * 函数名、类名和小括号之间不加空格,各种序列(元组、列表、字符串)和字典对象做索引运算时,对象名和中括号之间不加空格,例如class Monster():,get_width()，monsters[3];
> * 小括号和中括号的内侧不加空格,如(a + b),def init(int size):,npcs[npc_idx]，names = ["Jane", "Bill "];
> * 大括号内侧加一个空格，例如：d = { key: value }。

**4. 空行**

> * 每一个函数之间至少保留一个空行,每个类定义之间保留两个空行;
> * 在函数体内，逻辑相关紧密的代码行作为一个段落,段落间保留一个空行;
> * 不同种类模块的import语句之间保留一个空行.

**5. 断行**

> * 避免过长的代码行,最大长度不超过100个字符,如果过长应该在适当的位置换行,换行后多出一个TAB缩进;
> * 续行符“\”前要留一个空格.

**6. 模块导入（import）**

> * 多个模块如果关联紧密可以在一条import语句中导入,否则分开多条语句;
> * 先导入Python内置模块,再导入第三方模块,最后导入自己项目中的其他模块,几种模块间用空行分隔开;
> * 不要使用from module import *,除非是常量定义模块和确保不会出现命名空间冲突的模块.

**7. 分支和循环**

> * 不要将if语句和分支写成一行,例如：if x in range(10): print x不是好代码,“print x”应该另起一行并多一个TAB缩进;
> * 不要将for语句、while语句和循环体写成一行.

**8. 注释**

> * 要习惯写注释,英文中文皆可,只要表述准确,特别是接口和不易读懂的代码应做详细注释,同时避免无用的注释;
> * 注释符“#”后和注释内容之间留一个空格,使用“TODO:”标签标注以后会增加或完善的内容,例如：# TODO: 在此处添加镜头特效.


### 资料仅供学习参考，切勿用于商业用途！


