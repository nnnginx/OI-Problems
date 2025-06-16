# AT_abc216_c [ABC216C] Many Balls

## 题目描述

### 题意

有一个空盒子。

你可以以任意顺序执行以下两种操作任意次：

- 操作 $A$ ：往盒子里放入一个球。
- 操作 $B$ ：使盒子里球的数量翻倍。

请输出一种**操作次数不超过 $120$ 的方案**使得盒子里有 $N$ 个球。

可以证明一定存在合法方案。

## 输入格式

输入一个整数 $N$ 。

## 输出格式

输出一个由 `A` 和 `B` 组成的字符串 $S$ ， $S$ 的第 $i$ 个字符表示第 $i$ 次操作的种类。

$S$ **至多由 $120$ 个字符**组成。

---


### 样例解释1

盒子中球数的变化情况为 $0 \xrightarrow{A} 1 \xrightarrow{A} 2 \xrightarrow{B} 4 \xrightarrow{A} 5$ 。

---



### 样例解释2

盒子中球数的变化情况为 $0 \xrightarrow{B} 0 \xrightarrow{B} 0 \xrightarrow{A} 1 \xrightarrow{B} 2 \xrightarrow{B} 4 \xrightarrow{A} 5 \xrightarrow{A} 6 \xrightarrow{A} 7 \xrightarrow{B} 14$ 。


$\textsf{Translated by @\color{5eb95e}nr0728}.$

## 输入输出样例 #1

### 输入 #1

```
5
```

### 输出 #1

```
AABA
```

## 输入输出样例 #2

### 输入 #2

```
14
```

### 输出 #2

```
BBABBAAAB
```

## 说明/提示

- $1 \le N \le 10^{18}$
- 输入的所有数都是整数。

---