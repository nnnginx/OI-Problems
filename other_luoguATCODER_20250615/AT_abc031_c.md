# AT_abc031_c [ABC031C] 数列ゲーム

## 题目描述

高桥和青木用长度为N的数列S玩游戏。

游戏中，高桥和青木各进行一回合。

游戏按照以下规则进行：

	首先，高桥在数列中圈一个数字。
	然后，青木在高桥没圈的数字中圈一个。
	接着，留下圈中的数字以及它们之间的数字，去掉其它数字。留下的数列叫T。
	最后，在数列T中，从左开始奇数个数字的和为高桥的得分，偶数个数字为青木的得分。

青木在能圈的数字中，圈出能使他得到最多分数的数字。如果这样的数有多个，圈出最左的数字。

高桥知道青木的圈数方法。请求出高桥能得到的最大得分。

## 输入格式

按照以下标准格式输入。

	第一行输入整数N(2<=N<=50)，N是数列S的数字数量。
	第二行输入N个整数a1,a2,...,aN(-50<=ai<=50,1<=i<=50)，整数ai是数列S从左往右数第i个数字。

## 输出格式

用一行输出高桥的最大得分。

在输出的末尾加上换行

## 输入输出样例 #1

### 输入 #1

```
6
1 -3 3 9 1 6
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
3
5 5 5
```

### 输出 #2

```
10
```

## 输入输出样例 #3

### 输入 #3

```
8
-1 10 -1 2 -1 10 -1 0
```

### 输出 #3

```
-1
```