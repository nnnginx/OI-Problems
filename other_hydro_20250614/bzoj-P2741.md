

## 题目描述
FOTILE得到了一个长为 $N$ 的序列 $A$，为了拯救地球，他希望知道某些区间内的最大的连续 $\rm XOR$ 和。

即对于一个询问，你需要求出 
$$\max_{l\le i\le j\le r}\bigoplus_{k=i}^{j} a_k$$

为了体现在线操作，对于一个询问 $(x,y)$：
- $l = \min ( ((x+{\rm lastans}) \bmod N)+1 , ((y+{\rm lastans}) \bmod N)+1)$.
- $r = \max ( ((x+{\rm lastans}) \bmod N)+1 , ((y+{\rm lastans}) \bmod N)+1)$.

**其中 $\rm lastans$ 是上次询问的答案，一开始为0。** 
## 输入格式
第一行两个整数 $N$ 和 $M$。
第二行有 $N$ 个正整数，其中第 $i$ 个数为 $A_i$，有多余空格。
后M行每行两个数 $x,y$ 表示一对询问。
## 输出格式 
共 $M$ 行，第 $i$ 行一个正整数表示第 $i$ 个询问的结果。

```input1
3 3
1 4 3
0 1
0 1
4 3

```
```output1
5
7
7
```

## 提示
HINT
$N=12000$，$M=6000$，$x,y,A_i$ 在 `signed long int` 范围内。
## 题目来源
By seter


