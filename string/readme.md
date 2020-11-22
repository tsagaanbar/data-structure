# 串

## 串的概念

数据结构是指两个集合：

- a. 有特定关系的元素的集合（元素集）

- b. 这些元素之间的关系的集合（关系集） 

元素之间的关系有： 

- a. 线性关系

- b. 非线性关系 

在各种各样的数据结构中，如果其中的元素是线性关系，我们就称呼这个数据结构为**线性表**； 

如果**线性表**中的元素集是字符集（即元素类型均为字符型），我们就称这种线性表为**串**。



串的长度：串中所包含的字符个数称为该串的长度。

空串：长度为零，即不包含任何字符 

空格串（空白串）：所有字符都是空格

子串：串中任意个连续字符组成的子序列；并规定空串是任意串的子串。任意串是其自身的子串。



## 链串

通常将链串中每个节点所存储的字符个数称为**结点大小**。



## 串的模式匹配

串的模式匹配：在目标串`s`中查找与模式串`t`相等的子串。

KMP算法：

[如何更好地理解和掌握 KMP 算法? - 知乎 (zhihu.com)](https://www.zhihu.com/question/21923021)

[KMP 算法_经典算法与数据结构 - SegmentFault 思否](https://segmentfault.com/a/1190000008575379)

[字符串匹配的KMP算法 - 阮一峰的网络日志 (ruanyifeng.com)](http://www.ruanyifeng.com/blog/2013/05/Knuth–Morris–Pratt_algorithm.html)

[开篇词 - labuladong的算法小抄 (gitbook.io)](https://labuladong.gitbook.io/algo/)
