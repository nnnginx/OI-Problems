## 题目描述


俄罗斯方块是一款风靡全球的电视游戏机和掌上游戏机游戏，它由俄罗斯人阿列克谢·帕基特诺夫发明，故得此名。俄罗斯方块的基本规则是移动、旋转和摆放游戏自动输出的各种方块，使之排列成完整的一行或多行并且消除得分。由于上手简单、老少皆宜，从而家喻户晓，风靡世界。

俄罗斯方块共有以下七种，这些方块可以旋转但不能翻转。

![](./2772/file/pic1.jpg)

现在小 N 家中刚好要装修客厅，他希望使用俄罗斯方块来铺地板。小 N 家的地板大小为 $n \times m$。他想知道他共有多少种铺地板的方法。要求这些俄罗斯方块不能重叠，且要将地板刚好铺满。

另外在小 N 家的客厅中还有一些柱子，显然在柱子底下是不能铺地板的。

## 输入格式

第一行三个整数 $n,m,k$ 表示客厅长度、宽度和柱子数量。

之后的 $k$ 行，每行两个整数 $x,y$（$0 \leq x < n,0 \leq y < m$），表示柱子在第 $x$ 行第 $y$ 列。

## 输出格式

输出一个整数，表示方案数 $\text{mod} (10^9+7)$的值。

```input1
3 3 1
1 1
```

```output1
4
```

## 数据规模与约定

* 对于 $100\%$ 的数据，$k \leq n \times m$，$n \leq 30$，$M \leq 7$。

## 题目来源

插头Dp
