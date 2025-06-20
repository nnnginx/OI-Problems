# AT_abc308_g [ABC308G] Minimum Xor Pair Query

## 题目描述

这里有一块你可以写整数的黑板，初始黑板上什么都没有。

现在有 $q$ 个操作/询问，格式如下：

+ 操作 `1 x`：在黑板上写下一个数 $x$。
+ 操作 `2 x`：将**一个**整数 $x$ 从黑板上擦去，保证此时黑板上至少有一个整数 $x$。
+ 询问 `3`：输出黑板上任意两个整数的异或值的最小值，保证此时黑板上至少有两个数。

## 输入格式

第一行一个整数 $q$，表示操作/询问总数。

接下来 $q$ 行，每行一个操作，格式如上。

## 输出格式

对于每个询问 `3`，输出黑板上任意两个整数的异或值的最小值。

## 输入输出样例 #1

### 输入 #1

```
9
1 2
1 10
3
1 3
3
2 2
3
1 10
3
```

### 输出 #1

```
8
1
9
0
```

## 说明/提示

$1\leq q\leq 3\times 10^5,0\leq x<2^{30}$。


**对于样例 1：**

共有 9 个询问。

1. 此时黑板上有整数 $\{2\}$。
2. 此时黑板上有整数 $\{2,10\}$。
3. $2\oplus10=8$ 是黑板上最小的异或值。
4. 此时黑板上有整数 $\{2,3,10\}$。
5. $2\oplus3=1$ 是黑板上最小的异或值。
6. 此时黑板上有整数 $\{3,10\}$。
7. $3\oplus10=9$ 是黑板上最小的异或值。
8. 此时黑板上有整数 $\{3,10,10\}$。
9. $10\oplus10=0$ 是黑板上最小的异或值。

Translate by Ew_Cors.