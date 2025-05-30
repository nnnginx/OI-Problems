## 题目描述
Farmer Nhoj dropped Bessie in the middle of nowhere! At time $t=0$, Bessie is located at $x=0$ on an infinite number line. She frantically searches for an exit by moving left or right by $1$ unit each second. However, there actually is no exit and after $T$ seconds, Bessie is back at $x=0$, tired and resigned.

Farmer Nhoj tries to track Bessie but only knows how many times Bessie crosses $x=0.5,1.5,2.5,\cdots,(N−1).5$
, given by an array $A_0,A_1, \cdots ,A_{N−1} (1 \le N \le 10^5, 1 \le A_i \le 10^6)$. Bessie never reaches $x>N$ nor $x<0$.

In particular, Bessie's route can be represented by a string of $T=\sum\limits_{i=0}^{N-1}A_i$
Ls and Rs where the ith character represents the direction Bessie moves in during the ith second. The number of direction changes is defined as the number of occurrences of $LR$s plus the number of occurrences of $RL$s.

Please help Farmer Nhoj count the number of routes Bessie could have taken that are consistent with $A$
and minimize the number of direction changes. It is guaranteed that there is at least one valid route. 

## 输入格式
The first line contains $N$. The second line contains $A_0,A_1, \cdots ,A_{N−1}$. 

## 输出格式
The number of routes Bessie could have taken, modulo $10^9+7$. 

## 题目大意
#### 【题目描述】
现在有一条数轴，$t$ 表示当前时刻。在 $t=0$ 时 Bessie 恰好处在 $x=0$ 的位置。

接下来，每秒钟 Bessie 会向左或者向右移动一个单位距离，我们保证 Bessie 是在 $0-N$ 的位置之间移动并最终停在 $x=0$ 的位置。同时，我们有一个 $A_0,A_1,A_2\ldots A_{N-1}$ 的数列，分别表示 Bessie 经过 $0.5,1.5,2.5\ldots (N-1).5$ 这些点的次数。我们可以用一个由 $\text{L}$ 和 $\text{R}$ 组成的序列来表示 Bessie 的路径，我们称 Bessie 改变了一次方向为在序列中的相邻两个字符不同。现在我们不知道具体的移动序列是什么，但我们知道 Bessie 采用了让她改变方向次数最少的走法。现在请问 Bessie 的路径有多少种不同的可能情况？（我们称两条路径不同当且仅当这条路径对应序列中的某一位不同）

#### 【输入格式】
第一行一个正整数表示 $N$。

接下来一行有 $N$ 个用空格分隔的正整数表示 $A_0,A_1,A_2\ldots A_{N-1}$。

#### 【输出格式】
一行一个整数表示结果总数。由于这个值可能很大，请输出其对 $10^9+7$ 取模的结果。

#### 【数据范围】
$N\le10^5,\max(A_i)\le10^6$。

对于测试点 $2-4$，满足 $N\le2,\max(A_i)\le10^3$。

对于测试点 $5-7$，满足 $N\le2$。

对于测试点 $8-11$，满足 $\max(A_i)\le10^3$。

```input1
2
4 6
```

```output1
2
```

## 提示
### Explanation for Sample 1

Bessie must change direction at least 5 times. There are two routes corresponding to Bessie changing direction exactly 5 times: 

$\texttt{RRLRLLRRLL}$  
$\texttt{RRLLRRLRLL}$

### Scoring

 - Inputs $2-4$: $N \le 2$ and $\max(A_i) \le 10^3$
 - Inputs $5-7$: $N \le 2$
 - Inputs $8-11$: $\max(A_i) \le 10^3$
 - Inputs $12-21$: No additional constraints.

