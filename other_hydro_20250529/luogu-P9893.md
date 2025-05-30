## 题目描述
DreamGrid and BaoBao are playing a game.  There are $n$ soldiers in the game, numbered from $1$ to $n$. The $i$-th soldier has a power value of $a_i$. DreamGrid and BaoBao are going to divide the soldiers into several teams according to the rules below:

- A team must consist of 1 or 2 soldiers.
- Every soldier must belong to exactly 1 team.
- If a team consists of two soldiers (let's say they are the $i$-th and the $j$-th soldier), there must be $|i - j| = 1$.

The power value of a team is defined as the sum of the team members' power values. For the sake of fairness, they want to minimize the difference between the maximum team power value and the minimum team power value after the division. You are asked to find the minimum difference.



## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($1 \le n \le 10^5$), indicating the number of soldiers.

The second line contains $n$ integers $a_1, a_2, ... , a_n$ ($-10^9 \le a_i \le 10^9$), where $a_i$ indicates the power value of the $i$-th soldier.

It's guaranteed that the sum of $n$ in all test cases will not exceed $10^6$.


## 输出格式
For each test case output one line containing one integer, indicating the minimum difference between the maximum team power value and the minimum team power value.


## 题目大意
**DreamGrid** 和 **BaoBao** 在玩游戏。游戏中有 $n$ 个士兵，编号为 $1\sim n$。第 $i$ 名士兵的权利值为 $a_i$。**DreamGrid** 和 **BaoBao** 将按照以下规则将士兵分成几个小组:

- 一个队伍必须由 $1$ 或 $2$ 名士兵组成。

- 每个士兵必须只属于一个队伍。

- 如果一个团队由两名士兵 $i,j$ 组成，则必须有 $|i - j| = 1$。

团队的权力值被定义为队内士兵权力值的总和。

为了公平起见，他们希望最小化分区后的**最大团队力量值**与**最小团队力量值**之间的**差值**。你被要求找出最小的差值。

有多测。

$1\leq n\leq 10 ^ 5$，$|a_i|\leq 10 ^ 9$，$\sum n\leq 10 ^ 6$。

```input1
3
5
-1 4 2 1 1
4
1 3 2 4
1
7
```

```output1
1
2
0
```

## 提示
We now explain the first sample test case. All possible divisions are listed below.

| Division | Difference | Division | Difference |
| :-: | :-: | :-: | :-:|
|[-1], [4], [2], [1], [1] | 4 - (-1) = 5| [-1, 4], [2], [1], [1] | 3 - 1 = 2 |
| [-1], [4], [2], [1, 1] | 4 - (-1) = 5 | [-1], [4, 2], [1, 1] | 6 - (-1) = 7 |
| [-1], [4], [2, 1], [1] | 4 - (-1) = 5 |  [-1, 4], [2], [1, 1] | 3 - 2 = 1 |
| [-1], [4, 2], [1], [1] | 6 - (-1) = 7 | [-1, 4], [2, 1], [1] | 3 - 1 = 2 |


So the answer is $\min(5, 5, 5, 7, 2, 7, 1, 2) = 1$.

