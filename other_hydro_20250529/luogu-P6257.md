## 题目背景
### Warning: If you submit a malicious program, you will be banned.
### 警告：恶意提交本题将被封号。


## 题目描述
In the Royal Family, names are very important! As the Royal Historian you have been charged with analyzing the patterns in the names of the Royal Ladies in the realm.

There have been n Royal Ladies, for convenience numbered from 1 to $n$. The name of each Lady is anuppercase letter concatenated with the name of her mother. The exception is the Lady numbered 1, the
founder of the Royal Family, whose name is just a single uppercase letter.

For example, ENERYS could be the mother of AENERYS (as the name AENERYS consists of the single uppercase letter 'A' concatenated with ENERYS, which is her mother's name). Similarly, AENERYS could be the mother of DAENERYS and YAENERYS.

You are given the description of all the Royal Ladies. Your task is to determine, for certain interesting strings $s$, the number of Royal Ladies for whom s is a prefix of their name.

For example, consider Sample Input 1 below, with a Royal Line that goes straight from the founder S to AENERYS (through YS, RYS, ERYS, NERYS and ENERYS), with each Lady having exactly one daughter. Then AENERYS has two daughters—DAENERYS and YAENERYS, with the latter havingone daughter, RYAENERYS.

In such a family, RY is a prefix of the names of two ladies: RYS and RYAENERYS. E is a prefix of the names of ERYS and ENERYS. N is a prefix only of NERYS's name, while S is a prefix only of the nameof the founder, S. AY is not a prefix of any Royal Lady's name.


## 输入格式
The first line of input contains two integers $n$ and $k$, where $n$ $(1 \leq n \leq 10^6)$ is the total number of Royal Ladies and $k$ $(1 \leq k \leq 10^6)$ is the number of query strings.

Then follow n lines describing the Royal Ladies. The $i^{th}$ of these lines describes the Royal Lady numbered $i$, and contains an uppercase letter $c_i$ ('A'–'Z') and an integer $p_i$, where $c_i$ is the first letter of the name of Lady $i$, and $p_i$ $(p1 = 0$ and $1 \leq pi \lt i$ for $i \gt 1)$ is the number of her mother (or $0$, in the case
of the First Lady). All the names are unique.

The remaining $k$ lines each contain one nonempty query string, consisting only of uppercase letters. The sum of the lengths of the query strings is at most $10^6$.

## 输出格式
Output $k$ lines, with the $i^{th}$ line containing the number of Royal Ladies who have the $i^{th}$ query string as a prefix of their name.

## 题目大意
**题目描述**

众所周知，皇室家族的名字非常有讲究。而作为研究皇室的历史学家的你，最近接到了一个艰巨的任务——分析王国历史中所有皇室夫人的名字。

王国历史上有 $n$ 位皇室夫人，方便起见，我们将其从 $1$ 至 $n$ 编号。除了 $1$ 号夫人外，其余夫人的名字均为一个大写字母连接着她母亲的名字。而 $1$ 号夫人作为王国的首任王后，她的名字只有一个大写字母。

例如，由于 `AENERYS` 由 `A` 与 `ENERYS` 组成，因此 `ENERYS` 是 `AENERYS` 的母亲。相似地，`AENERYS` 是 `DAENERYS` 与 `YAENERYS` 的母亲。

你知道王国历史上所有皇室夫人的姓名与关系，而你需要完成的任务是，对于其他历史学家感兴趣的名字串 $s$，总共有多少位夫人的名字是以 $s$ 起始的。

例如在样例的皇室族谱中，`S` 至 `AENERYS` 的这一支（包含 `YS`、`RYS`、`ERYS`、`NERYS` 与 `ENERYS` 这几位夫人）均只有一位女儿。接下来 `AENERYS` 有两位女儿，分别是 `DAENERYS`，以及女儿是 `RYAENERYS` 的 `YAENERYS`。

在这个皇室家族内，有两位夫人的名字以 `RY` 起始，她们是 `RYS` 与 `RYAENERYS`。而 `ERYS` 与 `ENERYS` 均以 `E` 起始。名字以 `N` 起始的仅有一位夫人 `NERYS`。同样地，以 `S` 起始的仅有首位王后 `S`。而没有任何一位夫人的名字以 `AY` 起始。

**输入格式**

第一行有两个整数 $n,k$，分别代表王国历史上皇室夫人总数，以及其他历史学家感兴趣的名字串的个数。

接下来 $n$ 行描述所有皇室夫人的姓名与关系。第 $i+1$ 行描述第 $i$ 位夫人的资料 $c_i$ 与 $p_i$，其中字符 $c_i$ 表示她名字的首位字母，$p_i$ 为她母亲的编号。对于编号为 $1$ 的首位王后，$p_1=0$。所有夫人的名字均不重复。

接下来 $k$ 行，每行为一个大写字母构成的非空串，代表一个其他历史学家感兴趣的名字串。

**输出格式**

输出 $k$ 行，第 $i$ 行为一个整数，代表总共有多少位夫人的名字是以第 $i$ 个感兴趣的名字串起始的。

**数据范围**

$1\leq n\leq 10^6$，$1\leq k\leq 10^6$，$p_1=0$，特别地，对于 $1\lt i\leq n$，保证有 $1\leq p_i\lt i$。感兴趣的名字串总长不超过 $10^6$。

```input1
10 5
S 0
Y 1
R 2
E 3
N 4
E 5
A 6
D 7
Y 7
R 9
RY
E
N
S
AY
```

```output1
2
2
1
1
0
```

## 提示
Source: ICPC World Finals 2019.

