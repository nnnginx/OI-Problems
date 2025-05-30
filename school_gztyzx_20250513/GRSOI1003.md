## 题目背景

集训结束了。

## 题目描述

xiaosi4081 快乐地回宿舍收拾行李。但是他遇到了一些麻烦。

xiaosi4081 有两个行李箱，两个行李箱都是线性结构。而不能放进一号行李箱的东西可以全部堆放到另外一个行李箱。

但是 xiaosi4081 觉得放进一号行李箱的东西需要满足且只满足如下条件的一条：

* 对于第 $i$ 个放进行李箱的东西，它的重量必须小于之前所有放到**奇数位**的行李箱的重量，且大于所有放到**偶数位**的行李箱的重量。
* 对于第 $i$ 个放进行李箱的东西，它的重量必须小于之前所有放到**偶数位**的行李箱的重量，且大于所有放到**奇数位**的行李箱的重量。

形式化的说，如果设放进一号行李箱的物品序列的重量序列为 $x$ ，那么其要满足且只满足如下条件的一条：

1. $x_i > \max_{j\%2=1 ~and~ j <i} x_j$ 和 $x_i < \min_{j\% 2=0 ~and~ j <i}x_j$  同时成立
2. $x_i > \max_{j\% 2=0 ~and~ j <i}x_j$ 和 $x_i < \min_{j\% 2=1 ~and~ j <i}x_j$ 同时成立。

注：**xiaosi4081 希望一号行李箱不是空的**

xiaosi4081 想看看有多少种方案可以把东西放进行李箱。

特别的是，一号行李箱的第一个位置放什么都可以。

当然，xiaosi4081 可不希望求出来的方案数太大，他只需要知道方案数模 $10^9+7$ 的结果。

注意放置进一号行李箱序列的物品序列必须是行李序列的子序列。也就是说，行李放进一号行李箱序列的相对顺序与提供的 $a$ 序列的顺序一致。

## 输入格式

第一行一个整数 $n$ 表示行李数量。

接下来一行有 $n$ 个整数，第 $i$ 个整数 $a_i$ 表示第 $i$ 个行李的重量。

## 输出格式

一个数，表示方案数。

## 样例 #1

### 样例输入 #1

```
3
1 2 3
```

### 样例输出 #1

```
6
```

## 提示

$n \leq 5000,a_i \leq 10^{18}$

合法的放进一号行李箱的序列为 $\{1\},\{2\},\{3\},\{1~2\},\{1~3\},\{2~3\}$。

