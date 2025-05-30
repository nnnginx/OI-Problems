## 题目描述
**Note: The time limit for this problem in Python is 15s.  Other languages have the default time limit of 2s.**

Each of Farmer John's $N$ barns has selected a team of $C$ 
cows to participate in field day. The breed of every cow is
either a Guernsey or a Holstein.  

The difference between two teams is defined to be the number of positions $i$
($1 \leq i \leq C$) at which the breeds of the cows in the $i$ th positions
differ. For every team $t$ from $1 \ldots N$, please compute the maximum
difference between team $t$ and any other team.

## 输入格式
The first line contains $C$ and $N$.

The next $N$ lines each contain a string of length $C$ of `G`s and `H`s.  Each line
corresponds to a team.

## 输出格式
For each team, print the maximum difference.


## 题目大意
### 题目描述

**提示：本题的 Python 时限为 15s。其它语言默认 2s。**

Farmer John 的 $N$ 个牛棚都会选出包含 $C$ 只奶牛的队伍去参加户外聚会。所有奶牛的品种都只可能是根西牛（`G`）或荷斯坦奶牛（`H`）。

我们将两个奶牛队伍中，同一位置对应的两头奶牛品种不同的所有位置 $i(1 \leq i \leq C)$ 的个数，定义为的两个奶牛队伍的差异。对于编号 $1...N$ 的每个奶牛队伍 $t$，请计算出 $t$ 和其它所有队伍的差异的最大值。

### 输入格式

第一行包含两个整数 $C$ 与 $N$。

接下来 $N$ 行，每行有一个长度为 $C$ 的，仅包含字母 `G` 和 `H` 的字符串，每行对应一支奶牛队伍。

### 输出格式

对于每个队伍，输出差异最大值。

### 说明/提示

第一个和第三个队伍的差异为 $5$。第二个和第三个队伍的差异为 $3$。

$2 \leq N \leq 10^5,1 \leq C \leq 18$。

- 对于测试点 2-5：$C = 10$。
- 对于测试点 6-9：所有答案最少为 $C - 3$。
- 对于测试点 10-20：没有额外条件。

```input1
5 3
GHGGH
GHHHH
HGHHG
```

```output1
5
3
5
```

## 提示
The first and third teams differ by $5$. The second and third teams differ by
$3$.

$2\le N\le 10^5$, $1\le C\le 18$.

- Inputs 2-5: $C = 10$.
- Inputs 6-9: All answers are at least $C-3$.
- Inputs 10-20: No additional constraints.

