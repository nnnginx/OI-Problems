## 题目描述
Farmer John's $N$ cows ($3 \leq N \leq 50,000$) are all located at distinct positions in his two-dimensional field.  FJ wants to enclose all of the cows with a rectangular fence whose sides are parallel to the x and y axes, and hewants this fence to be as small as possible so that it contains every cow (cowson the boundary are allowed).

FJ is unfortunately on a tight budget due to low milk production last quarter.He would therefore like to enclose a smaller area to reduce maintenance costs,and the only way he can see to do this is by building two enclosures instead of one.  Please help him compute how much less area he needs to enclose, in total,by using two enclosures instead of one. Like the original enclosure, the two enclosures must collectively contain all the cows (with cows on boundaries allowed), and they must have sides parallel to the x and y axes.  The two enclosures are not allowed to overlap -- not even on their boundaries. Note that enclosures of zero area are legal, for example if an enclosure has zero width and/or zero height.

## 输入格式
The first line of input contains $N$.  The next $N$ lines each contain two integers specifying the location of a cow. Cow locations are positive integers in the range $1 \ldots 1,000,000,000$.

## 输出格式
Write a single integer specifying amount of total area FJ can save by using two enclosures instead of one.

## 题目大意
### 题目描述

Farmer John 的 $N$ 头奶牛（$3 \leq N \leq 50,000$）位于他二维牧场的不同位置。FJ 想要用一个与 x 轴和 y 轴平行的矩形围栏将所有奶牛围住，并且他希望这个围栏尽可能小，以便它包含每一头奶牛（允许奶牛位于边界上）。

由于上季度牛奶产量低，FJ 的预算紧张。因此，他希望围住更小的区域以减少维护成本，而他唯一能想到的方法就是建造两个围栏而不是一个。请帮助他计算使用两个围栏而不是一个围栏总共可以减少多少面积。与原始围栏一样，这两个围栏必须共同包含所有奶牛（允许奶牛位于边界上），并且它们的边必须与 $x$ 轴和 $y$ 轴平行。这两个围栏不允许重叠——即使在它们的边界上也不行。注意，零面积的围栏是合法的，例如如果一个围栏的宽度和/或高度为零。

### 输入格式

输入的第一行包含 $N$。接下来的 $N$ 行每行包含两个整数，指定一头奶牛的位置。奶牛的位置是 $1 \ldots 1,000,000,000$ 范围内的正整数。

### 输出格式

输出一个整数，表示 FJ 通过使用两个围栏而不是一个围栏总共可以减少的面积。

```input1
6
4 2
8 10
1 1
9 12
14 7
2 3
```

```output1
107
```

