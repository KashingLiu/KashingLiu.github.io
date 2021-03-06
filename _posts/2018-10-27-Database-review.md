---
layout:     post                    # 使用的布局（不需要改）
title:      数据库系统复习            # 标题
subtitle:   Hello World, Hello Blog # 副标题
date:       2018-10-20              # 时间
author:     刘家成                   # 作者
header-img: img/post-bg-2015.jpg    # 这篇文章标题背景图片
catalog: true                       # 是否归档
tags:                               # 标签
    - 学习
---

<font color=#ff0000>域</font>：是一组具有相同数据类型的值的集合  
<font color=#ff0000>域的基数</font>：一个域允许取不同的值的个数  
笛卡尔积的基数是基数的乘积  
n目关系有n个属性  
关系的笛卡尔积的目数是各关系目数的和  


外模式/模式 -- > 逻辑独立性  
模式/内模式 -- > 物理独立性  

<font color=#ff0000>候选码</font>：某一属性组能唯一标识一个元组，**但其子集不能**    
<font color=#ff0000>主码</font>：候选码中选择某一个作为主码  
<font color=#ff0000>外码</font>：设F是关系R的一个或一组属性**但不是**R的码，K<sub>s</sub>是基本关系S的主码。  
　　　F和K<sub>s</sub>必须定义在同一个域。  
<font color=#ff0000>主属性</font>：候选码中的属性就是主属性  
如果有一个关系R( a, b, c, d, e )，ab合在一起作为一个候选码、c是另外一个候选码，则abc都是R的主属性  
关系模式由**关系名**、**属性名集合**、**属性来自的域**、**属性向域的映射**组成  
关系数据库的型也称为关系型数据库的模式，是对数据库的描述  
<font color=#ff0000>基本操作</font>：选择、投影、并、差、笛卡尔积  
结果都是**集合**  
？？？ER图与关系模型之间的转换  
？？？关系和SQL的转换

####关系完整性  
<p>其中实体完整性和参照完整性称为关系的两个不变性</p>

* <font color=#ff0000>实体完整性</font>（保证每个元组是可区分的）  
  属性或属性组A是基本关系R的主属性，则A中任一属性不能取空
* <font color=#ff0000>参照完整性</font>  
  参照关系R的外键指向了被参照关系S的主键（外码引用主码）  
  若属性F是关系R的外码，其与关系S的主码K<sub>s</sub>对应，则对R中F的取值规定：
  * F可以取空值
  * F可以等于关系S中某个主码的值  
  如学生和系，学生刚来的时候没有系可以是空值，但是若有系则必须属于系中的某个主码
* <font color=#ff0000>用户定义完整性</font>  

####关系代数
