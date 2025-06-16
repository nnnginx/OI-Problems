# AT_jag2017autumn_a Window

## 题目描述

### 题目大意
有$N$ 块自西向东的窗格。每个窗格的宽度为 $W$，高度为 $H$。从西面开始的第 $i$ 块窗格覆盖了从窗户西边缘开始的 $W\times (i-1)$ 和 $W\times i$ 之间的水平范围。有 $N$ 个关于如何滑动窗玻璃的指示$x_1,x_2,x_3,...x_N$， $x_i\leq W$。对于第 $i$ 个玻璃窗，若 $i$ 为奇数，则将第 $i$ 个玻璃向东滑动 $x_i$，否则将第 $i-1$ 个玻璃窗向西滑动 $x_i$ 。求最后窗口打开的面积。

## 输入格式

$N,H,W,x_1,x_2,...,x_n$。

## 输出格式

一行，表示最后窗口打开的面积。

### 详例

输入：
```
4 3 3
1 1 2 3
```

输出：

```
9
```

解释:

![](https://img.atcoder.jp/jag2017autumn/e4aefb46f2ffb88ee7acb623ccf10830.png)


Translated by [yuanzongzi799](https://www.luogu.com.cn/user/1176727).