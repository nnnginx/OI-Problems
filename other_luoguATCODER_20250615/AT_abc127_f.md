# AT_abc127_f [ABC127F] Absolute Minima

## 题目描述

有一个函数 $f(x)$ ，初始时 $f(x)=0$

接下来你会对这个函数进行 $Q$ 次以下操作：

- $\texttt{1 a b}$，将 $f(x)$ 替换为 $g(x)=f(x)+|x-a|+b$
- $\texttt{2}$，询问最小的整数 $x$ ，使得  $f(x)$ 取到最小值，以及 $f(x)$ 的最小值

## 输入格式

第一行一个整数 $Q$

接下来 $Q$ 行，每行一个或三个整数，表示一次操作。

## 输出格式

对于每一次询问，输出一行两个整数，分别表示最小的整数 $x$ ，使得 $f(x)$ 取到最小值，和 $f(x)$ 的最小值

## 输入输出样例 #1

### 输入 #1

```
4
1 4 2
2
1 1 -8
2
```

### 输出 #1

```
4 2
1 -3
```

## 输入输出样例 #2

### 输入 #2

```
4
1 -1000000000 1000000000
1 -1000000000 1000000000
1 -1000000000 1000000000
2
```

### 输出 #2

```
-1000000000 3000000000
```

## 说明/提示

$1 \le Q \le 200000,-10^9 \le a,b \le 10^9$ ，保证第一次操作一定是修改操作