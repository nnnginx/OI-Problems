## 题目描述
There are initially $N-1$ pairs of friends among FJ's $N$ cows labeled $1\dots N$, forming a tree. The cows are
leaving the farm for vacation one by one. On day $i$, the $i$ th cow leaves the
farm, and then all pairs of the $i$ th cow's friends still present on the farm
become friends. 

For each $i$ from $1$ to $N$, just before the $i$ th cow leaves,  how many
ordered triples of distinct cows $(a,b,c)$ are there such that none of $a,b,c$
are on vacation, $a$ is friends with $b$, and $b$ is friends with $c$?

## 输入格式
The first line contains $N$.

The next $N-1$ lines contain two integers $u_i$ and $v_i$ denoting that cows
$u_i$ and $v_i$ are initially friends.

## 输出格式
The answers for $i$ from $1$ to $N$ on separate lines.

## 题目大意
### 题目描述

最初，农夫 John 的 $N$ 头编号为 $1 \dots N$ 的奶牛中有 $N-1$ 对朋友关系，形成一棵树。奶牛们依次离开农场去度假。在第 $i$ 天，第 $i$ 头奶牛离开农场，然后所有仍在农场中的第 $i$ 头奶牛的朋友之间会成为朋友。

对于每个 $i$ 从 $1$ 到 $N$，在第 $i$ 头奶牛离开之前，有多少个有序三元组 $(a, b, c)$ 满足以下条件：$a, b, c$ 均未离开农场，$a$ 与 $b$ 是朋友，且 $b$ 与 $c$ 是朋友？

### 输入格式

第一行包含 $N$。

接下来的 $N-1$ 行，每行包含两个整数 $u_i$ 和 $v_i$，表示奶牛 $u_i$ 和 $v_i$ 最初是朋友。

### 输出格式

输出 $N$ 行，第 $i$ 行表示在第 $i$ 头奶牛离开之前的答案。

### 提示

对于第一个样例：  
- 在第 $1$ 头奶牛离开之前，三元组为 $(1, 2, 3)$ 和 $(3, 2, 1)$。  
- 在第 $1$ 头奶牛离开后，剩下的奶牛少于 $3$ 头，因此没有三元组。

对于第二个样例：  
- 最初，奶牛 $1$ 与所有其他奶牛是朋友，而其他奶牛之间没有朋友关系，因此三元组为 $(a, 1, c)$，其中 $a, c$ 是 $\{2, 3, 4\}$ 中的不同奶牛，共有 $3 \cdot 2 = 6$ 个三元组。  
- 在第 $1$ 头奶牛离开后，剩下的三头奶牛彼此都是朋友，因此三元组为这三头奶牛的任意排列，共有 $3! = 6$ 个三元组。  
- 在第 $2$ 头奶牛离开后，剩下的奶牛少于 $3$ 头，因此没有三元组。  

$2 \le N \le 2 \cdot 10^5$，$1 \le u_i, v_i \le N$。

- 输入 4-5：$N \le 500$。
- 输入 6-10：$N \le 5000$。
- 输入 11-20：没有额外限制。

```input1
3
1 2
2 3

```

```output1
2
0
0

```

```input2
4
1 2
1 3
1 4

```

```output2
6
6
0
0

```

```input3
5
3 5
5 1
1 4
1 2

```

```output3
8
10
2
0
0

```

## 提示
For the first sample:  
$(1,2,3)$ and $(3,2,1)$ are the triples just before cow $1$ leaves.  
After cow
$1$ leaves, there are less than $3$ cows left, so no triples are possible.

For the second sample:  
At the beginning, cow $1$ is friends with all other cows, and no other pairs of
cows are friends, so the triples are $(a, 1, c)$ where $a, c$ are different cows
from $\{2, 3, 4\}$, which gives $3 \cdot 2 = 6$ triples.  
After cow $1$ leaves, the remaining three cows are all friends, so the triples
are just those three cows in any of the $3! = 6$ possible orders.  
After cow $2$ leaves, there are less than $3$ cows left, so no triples are
possible.  

$2\le N\le 2\cdot 10^5$, $1\le u_i,v_i\le N$.

- Inputs 4-5: $N\le 500$.
- Inputs 6-10: $N\le 5000$.
- Inputs 11-20: No additional constraints.


