# AT_tenka1_2014_qualB_b エターナルスタティックファイナル

## 题目描述

## 题意
小A通过组合他所学的短语来吟唱咒语。

同一个短语可以在诵读咒语的过程中使用多次。

例如，如果你记住了 $aaa$、$bbb$ 和 $ccc$ 三个短语，你就可以念出 $aaaccc$、$aaabbb$ 和 $cccaaaaaa$ 这样的咒语。

小A不确定他是否能够通过组合他所记住的短语来吟唱他所要学习的新咒语。

为小A创建一个程序，计算有多少种短语的排列组合可以构建他所要学习的新咒语。

变化的数量可能很大，所以输出对 $10^9+7$ 取模后的结果。

## 输入格式

在第一行中，给出小A已经记住的短语的数量 $N$（$1 \le N \le 100$）。

在第二行，给出小A想记住的咒语 $S$。

$S$ 的长度，$|S|$，满足 $1 \le |S| \le 1000$ 且 $S$ 由小写字母组成。

第 $3$ 至第 $N$ 行给出了智明已经记住的短语 $T_i$。

$T_i$ 的长度，$|T_i|$，满足 $1 \le |T_i| \le 1000$ 且 $T_i$ 由小写字母组成。

PS：如果 $i \neq j$，则 $Ti \neq Tj$。

## 输出格式

用这 $n$ 个短语构成的 $S$ 的方案数，对 $10^9+7$ 取模

## 输入输出样例 #1

### 输入 #1

```
3
eternalstaticfinal
eternal
static
final
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
5
eternalstaticfinal
eternal
static
final
fin
al
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
5
abcdef
abc
def
abcdef
d
ef
```

### 输出 #3

```
3
```

## 输入输出样例 #4

### 输入 #4

```
5
aaaa
a
aa
aaa
aaaa
b
```

### 输出 #4

```
8
```

## 输入输出样例 #5

### 输入 #5

```
10
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
a
aa
aaa
aaaa
aaaaa
aaaaaa
aaaaaaa
aaaaaaaa
aaaaaaaaa
aaaaaaaaaa
```

### 输出 #5

```
146491918
```