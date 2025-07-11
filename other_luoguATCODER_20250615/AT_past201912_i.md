# AT_past201912_i 部品調達

## 题目描述

有 $m$ 个数列，对于每个数列，给出一个长为 $n$ 的字符串 $s_i$ 表示 $1$ 到 $n$ 之间的整数是否在第 $i$ 个数列中出现了（用`Y`表示“是”，用`N`表示“否”；字符串下标从 $1$ 开始）。每个数列都有一个选择的代价 $c_i$。

请选择若干个数列，使得将这些数列拼接后，$1$ 到 $n$ 之间的每一个整数都在拼接后的数列中出现。输出所选择的数列的代价之和的最小值。

## 输入格式

第一行为两个整数 $n$ 和 $m$。

接下来 $m$ 行，每行一个长为 $n$ 且仅含`Y`和`N`的字符串 $s_i$ 以及选择代价 $c_i$。

## 输出格式

若目标可达成，请输出最小代价之和；否则，输出`-1`。

### 数据规模与约定

$1 \le n \le 10$，$1 \le m \le 1000$，$1 \le c_i \le 10^9$，上述数值均为整数。

## 输入输出样例 #1

### 输入 #1

```
3 4
YYY 100
YYN 20
YNY 10
NYY 25
```

### 输出 #1

```
30
```

## 输入输出样例 #2

### 输入 #2

```
5 4
YNNNN 10
NYNNN 10
NNYNN 10
NNNYN 10
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
10 14
YNNYNNNYYN 774472905
YYNNNNNYYY 75967554
NNNNNNNNNN 829389188
NNNNYYNNNN 157257407
YNNYNNYNNN 233604939
NYYNNNNNYY 40099278
NNNNYNNNNN 599672237
NNNYNNNNYY 511018842
NNNYNNYNYN 883299962
NNNNNNNNYN 883093359
NNNNNYNYNY 54742561
NYNNYYYNNY 386272705
NNNNYYNNNN 565075143
NNYNYNNNYN 123300589
```

### 输出 #3

```
451747367
```