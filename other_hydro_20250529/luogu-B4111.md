## 题目描述
JOI 君喜欢做铜锣烧。

有 $N$ 种馅料和 $M$ 种皮，第 $i(1\leq i\leq N)$ 种馅料的美味值为 $a_i$，第 $j$ 种皮的美味值为 $b_j$。用第 $i$ 种馅料和第 $j$ 种皮做成的铜锣烧的美味值为 $(a_i+b_j)\times \max(a_i,b_j)$，其中 $\max(x,y)$ 表示 $x$ 和 $y$ 中的较大值。

求所有的 $N\times M$ 种铜锣烧的美味值之和。

## 输入格式
第一行输入两个正整数 $N,M$。

第二行输入 $N$ 个正整数 $a_1,a_2,\ldots,a_N$。

第三行输入 $M$ 个正整数 $b_1,b_2,\ldots,b_M$。

## 输出格式
一行一个整数，表示答案。

```input1
2 2
1 2
2 5
```

```output1
79
```

```input2
1 5
50
9 7 5 4 1
```

```output2
13800
```

```input3
15 5
5 10 52 31 14 16 19 1 9 20 80 19 11 34 72
20 2 4 9 19
```

```output3
116756
```

## 提示
### 样例解释

对于样例 1，有四种铜锣烧，美味值分别为 $6,30,8,35$，和为 $79$。

### 数据范围 

$1\leq N\leq 100$，$1\leq M\leq 100$。对于任意 $i$ 满足$1\leq i\leq N$，$1\leq a_i\leq 100$。对于任意 $j$ 满足 $1\leq j\leq M$，$1\leq b_i\leq 100$。

