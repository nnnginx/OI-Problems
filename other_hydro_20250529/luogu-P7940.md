## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/zshuq5iq.png)

## 题目描述
**The difference between the versions is the limit of operations.**

Alice is a cute girl who has a lot of dolls.

There are $4\cdot n$ dolls playing *rock-paper-scissors*. They are divided into two teams: Team A and Team B. Each team contains $2\cdot n$ dolls.

A total of $2\cdot n$ rounds of the game will be played. In the $i$-th round, the $i$-th doll in Team A will play against the $i$-th doll in Team B. If the doll in Team A wins, Team A will get $1$ point. If it loses, Team A will lose $1$ point. If it ties, Team A will not get points.

Alice knows all the dolls' choices in this game. To be precise, she uses two arrays $a$ and $b$ to represent the choices of the dolls in the two teams. $a_i$ means the choice of the $i$-th doll in Team A, and $b_i$ means the choice of the $i$-th doll in Team B. In this question, we use $1$ for rock, $2$ for scissors, and $3$ for paper.

Now for **each team**, Alice wants to change the choices of **exact** $n$ dolls to make the score of Team A as high as possible.

Find the maximum score of Team A and its construction method. If there are multiple answers print any of them (you still have to maximize the score of Team A).

## 输入格式
Each test contains multiple testcases. The first line contains an integer $T$, the number of test cases.

For each test case, the first line contains one integer $n$.

Then two lines follow, containing an array $a$ of length $2\cdot n$ and an array $b$ of length $2\cdot n$, respectively.

## 输出格式
For each test case, output three lines.

The first line contains one integer, which is the maximize the score of Team A.

The second line contains an array $a'$ of length $2\cdot n$, which represents the modified $a$ array. For integers $1$ to $2\cdot n$, if $a_i \ne a'_i$, then it means you have modified the hand shape of one player in Team A.

The third line contains an array $b'$ of length $2\cdot n$, which represents the modified $b$ array. For integers $1$ to $2\cdot n$, if $b_i \ne b'_i$, then it means you have modified the hand shape of one player in Team B.

## 题目大意
AB 每队 $2n$ 人正在玩石头剪刀布。A 队第 $i$ 个人出 $a_i$，B 队第 $i$ 个人出 $b_i$。编号相同的人会对战。若 A 队赢则加一分，平不得分，输扣一分。你必须**恰好**改变**每队** $n$ 个人的出拳方案，使得 A 队的得分最高。输出得分的最大值和任意一组构造方案。

本题中，我们用 $1$ 代表石头，$2$ 代表剪刀，$3$ 代表布。

```input1
1
1
1 2
1 2
```

```output1
2
1 1
2 2
```

## 提示
### Explanation

For the first test case, we can change $a_2$ to $1$ and $b_1$ to $2$. Then Team A can get $2$ points. It can be proved that this is the maximum score that Team A can get.

### Constraints

$1\le T,n \le 10^5;\ 1\le a_i,b_i \le 3$. The sum of $n$ of all test cases $\le 10^5$.

