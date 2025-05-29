## 题目描述

在膜拜 sone 神题之余，Stilwell 决定出一道福利题。

Stilwell 等弱菜开始讨论矩阵的问题：

> Memphis：矩阵加减不是特水，矩阵求和显然是应该有的
> 
> WWT:轴对称变换，平移操作不是超有趣
> 
> YZH：单点修改也加上
> 
> LY：可以把矩阵输出玩一下
> 
> Stilwell：旋转操作不是挺逗
> 
> ……

最后，Stilwell 等人发现自己太弱了，于是请花老师秒出了标程。

## 输入格式

第一行是一个整数 $n$ ，表示有一个 $n\times n$ 的矩阵。

从输入数据的第二行开始到文件尾的每一行会出现以下几种操作：

|操作|参数|内容|
|:--:|:--:|:--:|
|$L$|$a\ b\ c\ d\ delta$|将 $(a,b),(c,d)$ 为顶点的矩形区域内的所有数字加上 $delta$|
|$k$|$a\ b\ c\ d$|代表求 $(a,b),(c,d)$ 为顶点的矩形区域内所有数字的和|
|$Fx$|/|将这个图形绕 $x$ 轴中心翻转，例： $\begin{bmatrix}1&2&3\\4&5&6\\7&8&9\end{bmatrix} \rightarrow \begin{bmatrix}3&2&1\\6&5&4\\9&8&7\end{bmatrix}$|
|$Fy$|/|将这个图形绕 $y$ 轴中心翻转，例： $\begin{bmatrix}1&2&3\\4&5&6\\7&8&9\end{bmatrix} \rightarrow \begin{bmatrix}7&8&9\\4&5&6\\1&2&3\end{bmatrix}$|
|$Dx$|$a$（可能为负）|将这个图形沿 $x$ 轴平移 $a$ 个单位，例： $\begin{bmatrix}1&2&3\\4&5&6\\7&8&9\end{bmatrix} \rightarrow \begin{bmatrix}7&8&9\\1&2&3\\4&5&6\end{bmatrix}(a=1)$|
|$Dy$|$a$（可能为负）|将这个图形沿 $y$ 轴平移 $a$ 个单位，例： $\begin{bmatrix}1&2&3\\4&5&6\\7&8&9\end{bmatrix} \rightarrow \begin{bmatrix}3&1&2\\6&4&5\\9&7&8\end{bmatrix}(a=1)$|
|$R+$|/|将这个图形顺时针旋转$90\degree$，例： $\begin{bmatrix}1&2&3\\4&5&6\\7&8&9\end{bmatrix} \rightarrow \begin{bmatrix}7&4&1\\8&5&2\\9&6&3\end{bmatrix}$|
|$R-$|/|将这个图形逆时针旋转$90\degree$，例： $\begin{bmatrix}1&2&3\\4&5&6\\7&8&9\end{bmatrix} \rightarrow \begin{bmatrix}3&6&9\\2&5&8\\1&4&7\end{bmatrix}$|
|$C$|$a\ b\ delta$|将点 $(a,b)$ 的值改为 $delta$|
|$Q$|/|将当前的整个矩阵输出|

请注意，沿用 `上帝造题的七分钟` ， $k$ 为小写。

注：读入矩阵时，第 $i$ 行第 $j$ 个表示坐标 $(x,y)$ 为 $(i,j)$ 的点。

## 输出格式

对于每一个 $k$ ，在单独一行输出一个答案。

对于每一个 $Q$ ，输出整个矩阵。

## 样例输入

```plain
2
L 1 1 1 1 1
L 1 2 1 2 2
L 2 1 2 1 3
L 2 2 2 2 3
C 2 2 4
Fx
Rk 1 2 2 2
Dy 1
k 1 2 2 2
Q
```

## 样例输出

```plain
7
3
3 1
4 2
```

## 数据规模与约定

对于 $100\%$ 的数据， $1\le n\le 1024 , |delta| \le 100$ ，操作不超过 $ 2\times10^5$ 个，保证运算过程中及最终结果均不超过 32位带符号整数类型 的表示范围，保证 $Q$ 操作总数不超过 $3\times10^3$ 。

