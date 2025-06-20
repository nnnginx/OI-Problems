# AT_tkppc6_2_f Shortest Path Construction

## 题目描述

[**problemURL**](https://atcoder.jp/contests/tkppc6-2/tasks/tkppc6_2_f)

F君正在解一道题：
>P国由 $N$ 个街道和 $M$ 条道路组成，道路 $i$ 连接街道 $A_i$ 和街道 $B_i$，通过时花费 $C_i$ 分钟。
>
>请求出从街道 $1$ 走到街道 $i$ 再走到街道 $N$ 所花费的总时间的最小值 $D_i$。允许多次通过同一顶点或道路。

F君知道每个 $D_i$，但是他忘记了 $A,B,C$ 是什么，请为他找出一组 $A,B,C$。

## 输入格式

第一行 $2$ 个正整数 $N,M$。  
第二行 $N$ 个正整数 $D_i$。

## 输出格式

若**存在**满足条件的 $A,B,C$：  
第一行 $1$ 个字符串`Yes`。  
接下来 $M$ 行，每行 $3$ 个正整数 $A_i,B_i,C_i$。  
若存在多组满足条件的 $A,B,C$，可以输出其中任意 $1$ 个。

若**不存在**满足条件的 $A,B,C$：  
$1$ 个字符串`No`。

输出需满足以下条件：
- $ 1\leq A_i<B_i\leq N(1\leq i\leq M) $。
- $ 0\leq C_i\leq 10^9(1\leq i\leq M) $。
- $ (A_i,B_i)\neq(A_j,B_j)(1\leq i<j\leq M) $。
- 必须走过超过 $0$ 条道路。
- 对于每个 $i$，$C_i$ 是整数。
## 【样例解释 1】
例如，第 $3$ 天花费时间最小的路径将依次通过道路 $2,6,7$
，花费的时间分别是 $2,3,1$，所以合计需要 $6$ 分钟。
## 【样例解释 3】
可以证明不存在满足条件的 $A,B,C$。

Translated by leozhao123

## 输入输出样例 #1

### 输入 #1

```
5 7
5 5 6 6 5
```

### 输出 #1

```
Yes
1 2 1
1 3 2
1 4 6
2 4 5
2 5 4
3 4 3
4 5 1
```

## 输入输出样例 #2

### 输入 #2

```
5 4
10 10 10 10 10
```

### 输出 #2

```
Yes
1 2 1
2 3 2
3 4 3
4 5 4
```

## 输入输出样例 #3

### 输入 #3

```
3 100
1 3 2
```

### 输出 #3

```
No
```