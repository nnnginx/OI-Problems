## 题目描述

有 $n$ 个工作，$m$ 种机器，每种机器你可以租或者买过来。

每个工作包括若干道工序，每道工序需要某种机器来完成。

现在给出这些参数，求最大利润。

## 输入格式

第一行两个整数 $n,m$。

下面将有 $n$ **块**数据，对于第 $i$ 块数据：

第一行给出 $w_i,k_i$ 表示完成这个任务能赚到的钱及有多少道工序。

接下来 $k_i$ 行每行两个数，分别描述完成工序所需要的机器编号 $id_{i,j}$ 及租用它的费用 $b_{id_{i,j}}$。

最后 $m$ 行，第 $i$ 行给出购买机器 $i$ 的费用 $b_i$。

## 输出格式

一行一个整数表示最大能获得的利润。


```input1
2 3
100 2
1 30
2 20
100 2
1 40
3 80
50
80
110
```


```output1
50
```

## 样例说明 

![](./941/file/pic1.jpg)

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n,m\leq1200$，$1\leq w_i\leq 5000$，$1\leq a_i,b_i\leq 2\times 10^4$。

