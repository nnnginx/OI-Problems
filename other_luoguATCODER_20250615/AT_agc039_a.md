# AT_agc039_a [AGC039A] Connection and Disconnection

## 题目描述

给定一个字符串 $S$，令 $T$ 为 $S$ 的 $K$ 个副本首尾相接得到的字符串。  
我们可以重复进行以下操作：选择 $T$ 中的一个字符并将其替换为另一个字符。  
请最小化能使得 $T$ 中任意相邻字符不相同的最少操作数。

## 输入格式

第一行，一个字符串 $S$。  
第二行，一个正整数 $K$。

## 输出格式

一行，表示最少操作数。

## 输入输出样例 #1

### 输入 #1

```
issii
2
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
qq
81
```

### 输出 #2

```
81
```

## 输入输出样例 #3

### 输入 #3

```
cooooooooonteeeeeeeeeest
999993333
```

### 输出 #3

```
8999939997
```

## 说明/提示

### 数据限制
- $1 \le |S| \le 100$。
- $S$ 仅由小写字母组成。
- $K \in [1,10^9] \bigcap \mathbb Z$。

### 样例解释 1
$T = \texttt{issiiissii}$。  
一种可行的方案是将其改写为 $\texttt{ispiqisyhi}$，此时任意相邻字符不相同。