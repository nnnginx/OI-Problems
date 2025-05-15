标题来自 [くうになる (feat. 可不&初音ミク)](https://music.163.com/song?id=1912598037&userid=3392731818)。

## 题目描述

芙宁娜有 $n$ 个字符串 $s_1,\cdots,s_n$。

现在芙宁娜想要从中选出字符串 $s_i,s_j,s_k,s_l$，并交换 $s_i,s_j$ 的一个前缀，使得交换完之后它们恰好分别是 $s_k,s_l$。形式化地，你需要找到四个字符串 $s_i,s_j,s_k,s_l$，然后你需要将 $s_i,s_j$ 划分为一个非空前缀和一个非空后缀，即 $s_i=A+B,s_j=C+D$（其中 $+$ 表示拼接），且满足 $A\neq C,B\neq D,s_k=C+B,s_l=A+D$。

例如，四个字符串分别是 $s_i=\texttt{abc},s_j=\texttt{def},s_k=\texttt{dc},s_l=\texttt{abef}$，考虑 $A=\texttt{ab},B=\texttt{c},C=\texttt{d},D=\texttt{ef}$，那么就有

$$
s_i=A+B,s_j=C+D,s_k=C+B,s_l=A+D
$$

于是这一组 $(i,j,k,l)$ 就符合要求。找到任意一组解即可，或报告无解。

注意这里只需要 $A\neq C,B\neq D$，并不要求 $i,j,k,l$ 互不相同。例如

```
bababb
bababb
baababb
bbabb
```

也是一组合法的 $s_i,s_j,s_k,s_l$（尽管 $s_i=s_j$）。其中 $A=\texttt{b},B=\texttt{ababb},C=\texttt{ba},D=\texttt{babb}$。

## 输入格式

**本题有多组数据。** 第一行一个正整数 $T$ 表示数据组数。对于每组数据：

第一行一个正整数 $n$ 表示字符串个数。

接下来 $n$ 行，每行一个仅由小写字母构成的字符串。

## 输出格式

对于每组数据：

若无解，输出一行一个字符串 `NO`。

否则，你首先需要输出 `YES`，然后输出六个正整数 $i,j,k,l,p,q$，表示你选择的字符串是 $s_i,s_j,s_k,s_l$，且 $A=s_i[1\cdots p],B=s_i[p+1\cdots L_i-1],C=s_j[1\cdots q],D=s_j[q+1\cdots L_j-1]$。

这里字符串的下标和字符串的编号从 $1$ 开始，$L_i$ 表示第 $i$ 个字符串的长度。你需要保证：

- $A\neq C,B\neq D$。
- $1\le p<L_i,1\le q<L_j$。
- $s_i=A+B,s_j=C+D,s_k=C+B,s_l=A+D$。

## 样例 $1$ 输入

```
3
5
abcdefzxcvbb
abc
def
abef
dc
5
jasdlkajdcpasjdcmasdpaxza
bababb
bababb
baababb
bbabb
4
adsd
sdjakdsl
ajsldla
asdlsajcp
```

## 样例 $1$ 输出

```
YES
3 2 4 5 1 2
YES
2 2 4 5 1 2
NO
```

## 测试点约束

设 $M$ 为一组数据中的字符串总长。

对于所有测试点，$4\le n,M\le 5\times 10^5$，且每个测试点中每组数据的 $n$ 之和与 $M$ 之和均不超过 $5\times 10^5$。

各子任务的详细信息见下表：

| 子任务编号 |        $n$         |        $M$         | 分值 | 依赖子任务 |
| :--------: | :----------------: | :----------------: | :--: | :--------: |
| Subtask #1 |      $\le 10$      |      $\le 50$      | $15$ |     无     |
| Subtask #2 |      $\le 20$      |     $\le 500$      | $10$ |    $1$     |
| Subtask #3 |     $\le 500$      |     $\le 500$      | $10$ |    $2$     |
| Subtask #4 |     $\le 2000$     |     $\le 2000$     | $10$ |    $3$     |
| Subtask #5 |     $\le 3000$     | $\le 5\times 10^5$ | $10$ |    $4$     |
| Subtask #6 | $\le 5\times 10^5$ | $\le 5\times 10^5$ | $45$ |    $5$     |

