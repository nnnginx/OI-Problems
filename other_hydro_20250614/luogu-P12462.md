## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/9eg0us72.png)

## 题目描述
星野阿库娅给了你一棵树 $T(V=\{V_1,V_2,\ldots,V_n\},E)$，树有边权 $\omega: E \mapsto \mathbb{Z^+}$。

定义 $S \subseteq E$ 的权值为 $\omega(S)=\sum_{e \in S} \omega(e)$。

定义 $R(V',E')$ 是 $T$ 的 $\textbf{连通子树}$，当且仅当 $R$ 是树，$V' \subseteq V$，$E' \subseteq E$。

定义 $R$ 的权值 $\omega(R)=\omega(E')$。

定义 $S \subseteq V$ 的 Steiner 树为 $f(S)=\min \{\omega(R) | S \subseteq V'\}$，其中 $R(V',E')$ 是连通子树。

有 $q$ 次询问，第 $i$ 次给出 $L_i,R_i,k_i$，求 $\max \{f(S) | S \subseteq \{V_{L_i},V_{L_{i}+1},\ldots,V_{R_i}\},|S|=k_i\}$。

## 输入格式
第一行一个整数 $n$。

下面 $n-1$ 行，每行三个整数 $a,b,z$，表示 $(V_a,V_b) \in E$，且 $\omega[(V_a,V_b)]=z$。保证 $1 \le z \le 10^9$。

下面一行一个整数 $q$。

下面 $q$ 行，第 $i$ 行三个整数 $L_i,R_i,k_i$. 保证 $1 \le L_i \le L_i + k_i - 1 \le R_i \le n$。

## 输出格式
$q$ 行，每行一个整数表示答案。

```input1
10
1 2 2
2 3 3
3 4 2
1 5 7
2 6 7
4 7 1
1 8 3
4 9 6
7 10 4
10
5 10 5
4 9 6
10 10 1
2 6 3
6 9 3
6 9 4
7 9 2
1 3 2
1 7 3
3 8 3
```

```output1
35
31
0
21
23
24
16
5
22
22
```

## 提示
Idea：nzhtl1477，Solution：rushcheyo&nzhtl1477，Code：rushcheyo，Data：rushcheyo

本题采用子任务评测。

设 $K=\max\{k_i\}$。

对所有数据，保证 $1 \le n \le 3 \times 10^5,1 \le q \le 10^4,K \le 100$.

1. $n,q \le 10$（15 分）；

2. $n,q \le 100$（15 分）；
3. $n,q \le 1000$（10 分）；
4. $n,q \le 5000$（10 分）；
5. $K=2$（15 分）；
6. $K=3$（15 分）；
7. $K \le 10$（10 分）；
8. 没有特殊性质（10 分）。

