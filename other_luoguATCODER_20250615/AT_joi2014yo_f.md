# AT_joi2014yo_f 小籠包 (Xiao Long Bao)

## 题目描述

## 题目大意
JOI再吃他的小笼包，第i个小笼包和第j个小笼包的距离是|i-j|。众所周知，吃小笼包时会把汁溅到别的小笼包上，吃第i个小笼包时，与第i个小笼包的距离在d[i]范围内的所有小笼包（不包括自己，包括距离刚好的d[i]的笼包）的味道会+1。吃到的笼包的味道=这个笼包本来的味道a[i]+这个笼包上的汁水。
现在JOI想知道，用怎么样的吃小笼包顺序可以让吃到的总味道最大。

## 输入格式

第1行是一个整数n（1<=n<=100),表示有n个笼包。
第2行有n个整数：D1、D2、D3...Dn(0<=Di<=7)，表示笼包会溅到的距离范围。
第3行有n个整数：A1、A2、A3...An(0<=Ai<=1000),表示笼包初始味道。

## 输出格式

输出最大的总味道。
## 输入输出样例：
![捕获.PNG](https://i.loli.net/2018/12/31/5c29e963e05fc.png)

样例1解释：吃的顺序：5->3->1->2->4

## 输入输出样例 #1

### 输入 #1

```
5
1 0 1 1 2
0 2 6 3 4
```

### 输出 #1

```
20
```

## 输入输出样例 #2

### 输入 #2

```
10
5 2 7 2 6 5 3 5 3 6
8 7 8 4 0 6 0 10 10 0
```

### 输出 #2

```
237
```