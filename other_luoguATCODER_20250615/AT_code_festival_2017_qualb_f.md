# AT_code_festival_2017_qualb_f Largest Smallest Cyclic Shift

## 题目描述

对于字符串 $S$，定义 $f(S)$ 为 $S$ 的所有循环移位中字典序最小的一个。例如，当 $S =$ `babca` 时，$S$ 的循环移位（`babca`, `abcab`, `bcaba`, `cabab`, `ababc`）中，字典序最小的是 `ababc`，因此 $f(S) =$ `ababc`。

给定三个整数 $X, Y, Z$，你需要构造一个包含恰好 $X$ 个字符 `a`，$Y$ 个字符 `b`，和 $Z$ 个字符 `c` 的字符串 $T$。如果有多个这样的字符串，你需要使得 $f(T)$ 在字典序上尽可能大。

求出 $f(T)$ 的字典序最大值。

## 输入格式

输入将以以下形式从标准输入中提供：

> $X$ $Y$ $Z$

## 输出格式

输出答案。

### 约束

- $1 \le X + Y + Z \le 50$
- $X, Y, Z$ 是非负整数。

### 样例解释 1

字符串 $T$ 必须由两个 `a` 和两个 `b` 构成。
- 当 $T =$ `aabb` 时，$f(T) =$ `aabb`。
- 当 $T =$ `abab` 时，$f(T) =$ `abab`。
- 当 $T =$ `abba` 时，$f(T) =$ `aabb`。
- 当 $T =$ `baab` 时，$f(T) =$ `aabb`。
- 当 $T =$ `baba` 时，$f(T) =$ `abab`。
- 当 $T =$ `bbaa` 时，$f(T) =$ `aabb`。

因此，$f(T)$ 的最大值是 `abab`。

---

Translated by User 735713.

## 输入输出样例 #1

### 输入 #1

```
2 2 0
```

### 输出 #1

```
abab
```

## 输入输出样例 #2

### 输入 #2

```
1 1 1
```

### 输出 #2

```
acb
```