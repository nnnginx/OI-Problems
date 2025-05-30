## 题目描述


Competitive programming is very popular in Byteland. In fact, every Bytelandian citizen is registered at two programming sites -- CodeCoder and TopForces. Each site maintains its own proprietary rating system. Each citizen has a unique integer rating at each site that approximates their skill. Greater rating corresponds to better skill.

People of Byteland are naturally optimistic. Citizen A thinks that he has a chance to beat citizen B in a programming competition if there exists a sequence of Bytelandian citizens $A = P_{0}, P_{1},...,P_{k} = B$ for some $k \ge 1$ such that for each $i (0 \le i < k) , P_{i}$ has higher rating than $P_{i+1}$ at one or both sites.

Each Bytelandian citizen wants to know how many other citizens they can possibly beat in a programming competition.



## 输入格式


The first line of the input contains an integer $n$ -- the number of citizens $(1 \le n \le 100 000)$ . $The following n$ lines contain information about ratings. The i-th of them contains two integers $CC_{i} and TF_{i}$ -- ratings of the i-th citizen at CodeCoder and TopForces $(1 \le CC_{i}, TF_{i} \le 10^{6}).$ All the ratings at each site are distinct.



## 输出格式


For each citizen $i$ output an integer $b_{i}$ -- how many other citizens they can possibly beat in a programming competition. Each $b_{i}$ should be printed in a separate line, in the order the citizens are given in the input.



## 题目大意
- 有 $n$ 个人，每个人有两个能力值 $CC_i$ 和 $TF_i$。第 $i$ 个人能打败第 $j$ 个人当且仅当 $CC_i >CC_j$ 或 $TF_i>TF_j$。

- 强的关系具有传递性，也就是说 $i$ 比 $j$ 强，$j$ 比 $k$ 强，那么 $i$ 比 $k$ 强。 求出每个人最多可以打败的人的个数。

- $n \leq10^5$，$CC_i,TF_i \leq10^6$，数据保证 $CC_i$ 两两不同、$TT_i$ 两两不同。

```input1
4
2 3
3 2
1 1
4 5

```

```output1
2
2
0
3

```

## 提示
Time limit: 2 s, Memory limit: 256 MB. 



