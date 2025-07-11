# AT_xmascon19_c Sokoban

## 题目描述

# Sokoban（推箱子）

## 题意翻译

小兔子的房间是一个有H行W列个格子的长方形。有三种格子，分别是“一般格子”、“目标位置格子”和“固定家具格子”。起初，小兔子和它的行李位于互不相同的“一般格子”上。

把从上往下数第i行，从左往右数第j列的格子记作$A_{i,j}$，一个格子可能出现以下几种状态：

* ` .`：空的一般格子
* `R`：小兔子的位置
* `a`：一般格子，上面有小兔子的行李
* `O`：目标位置格子，上面没有行李
* `@`：目标位置格子，上面有行李
* `#`：固定家具格子

小兔子想要将所有的行李都放到目标位置上。在接下来的每次行动中，它都可以选择以下两种行动方式中的一种执行：

* 走向它所在格子的上下左右个格子中的任意一个空的格子
* 走向它所在格子的上下左右个格子中的任意一个有行李的格子，同时行李向小兔子移动的方向移动一格

请求出小兔子最少的行动次数。

此外，该问题的所有输入文件都是公开的（请参照“评测”一段）

## 输入格式

共H+1行，第一行输入两个整数H,W

接下来的H行，每行输入W个字符，表示小兔子的房间

## 输出格式

输出最小的行动次数

## 输入输出样例 #1

### 输入 #1

```
6 7
#######
#R....#
#..@..#
###a###
###O###
#######
```

### 输出 #1

```
10
```

## 说明/提示

* $5 \leq H \leq 400$
* $5 \leq W \leq 400$
* $A_{i,j}$（$1 \leq  i \leq H,1 \leq  j \leq W$）是`.`,`R`,`a`,`O`,`@`和`#`中的一个。
* 输入数据中只有一个`R`
* 输入数据中`a`和`O`的数量相等，且多于一个
* 输入数据保证房间的边缘都是`#`
* 输入数据保证存在能将所有的行李都放到目标位置上的方法

## 评测

* 共有五个测试点，分别为`01.txt`,`02.txt`,`03.txt`,`04.txt`,`05.txt`，各个测试点占分不同，分别为7分，11分，17分，25分和40分。
* 在[此处](https://img.atcoder.jp/xmascon19/sokoban.zip)下载输入数据
* 你也可以实际操作小兔子在输入数据对应的房间中收视行李，[链接在这里](https://img.atcoder.jp/xmascon19/sokoban.html)（对应的html文件已包含在下载的输入数据中）

（顺便解释一下这个实操网站上的内容：这里面包含了样例，五个测试点的输入和一个附加房间（“omake”，不包含在输入数据中），用上下左右的方向键或者WASD又或是HJKL操作小兔子，网站中的“読み込み”是刷新的意思，“手数”是当前的步数，换地图后要点一下“読み込み”才会显示对应的房间)