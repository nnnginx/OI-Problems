## 题目描述
Mirko and Slavko like to hike together. Mirko likes mountain peaks, and Slavko likes valleys.
Because of this, every time they climb to a peak, Slavko decides which valley they are going
to descend to, given that a trail exists to it. Similarly, in each valley, Mirko decides which
peak they are going to climb up to. It will never be possible to directly climb from one peak to
another, or to get from one valley to another valley. In order to make the hiking as fun as
possible, they never visit the same spot twice (whether it’s a peak or a valley). Once they
reach a spot that only leads to spots they’ve visited before, they call the mountain rangers to
pick them up. If the final spot is a peak, Mirko wins, and if it is a valley, Slavko wins.

Naturally, you must already know what your task is: If we assume that both of them play
optimally, who wins? Answer this question for all initial peaks.

## 输入格式
The first line contains two positive integers, ​N and ​M (1 ≤ ​N ≤ 5000, 1 ≤ ​M ≤ min(5000, ​N
·​N
)).
Here ​N denotes the number of peaks and valleys (therefore, there are ​N peaks and ​N
valleys), and ​M
denotes the number of hiking trails.

Each of the following ​M lines contains two positive integers: ​$v_i$ and ​​$d_i$ (1 ≤ ​​$v_i$ , ​​$d_i$ ≤ ​N) that
denote there is a trail between peak ​​$v_i$ and valley ​$d_i$.
Between each peak and valley, there will exist at most one trail.

## 输出格式
You must output ​N
lines. The ​$i^{th}$ line denotes the winner if the starting point is peak ​i
.

## 题目大意
米尔科$(Mirko)$和斯拉夫科$(Slavko)$喜欢一起远足。米尔科喜欢山峰，斯拉夫科喜欢山谷。正因为如此，每当他们爬上一个山峰，若有连向山谷的路，则斯拉夫科就决定他们要去哪一个山谷。同样地，在每个山谷中，若有连向山峰的路，米尔科就决定他们将爬到哪一个山峰。不可能出现从一个山峰直接攀登到另一个山峰的情况，也不可能出现从一个山谷到另一个山谷的情况。为了使徒步旅行尽可能有趣，他们从不去同一地点两次（无论是一个山峰或一个山谷）。一旦他们到达一个地点，没有其它的地方可去，他们会叫登山者来接他们。如果最后一个点是一个山峰，则米尔科获胜，如果是一个山谷，则斯拉夫科获胜。

现在你的任务是，对于每一个山峰，如果他们从这里出发，并且都采用最优策略，谁会赢？

第一行两个正整数 $N,M$ $(1 ≤ N ≤ 5000, 1 ≤ M ≤ min(5000, N^2))$。$N$ 表示共有 $N$ 个山峰和 $N$ 个山谷。$M$ 表示共有 $M$ 条双向道路。

接下来 $M$ 行，每行两个正整数$v_i,d_i$ $(1 ≤ v_i,d_i≤ N)$ 表示第 $v_i$ 个山峰与第 $d_i$ 个山谷有路相连。

共 $N$ 行，每行一个字符串，第 $i$ 行表示从第 $i$ 个山峰出发的胜利者。

$30\%$的数据 $1 ≤ N≤ 10$

另有$20\%$的数据是森林。

```input1
2 3
1 2
2 2
2 1
```

```output1
Slavko
Slavko
```

```input2
4 5
2 2
1 2
1 1
1 3
4 2
```

```output2
Slavko
Mirko
Mirko
Mirko
```

```input3
4 5
1 2
1 3
2 2
2 3
4 1
```

```output3
Slavko
Slavko
Mirko
Slavko
```

## 提示
In test cases worth 30% of total points, it will hold 1 ≤ ​N
≤ 10 and 1 ≤ ​M
≤ ​N
·​N
.

In test cases worth an additional 20% of total points, for each two connected spots, there will
exist a unique path between them. In other words, the graph will be a forest.

**Clarification of the second test case:**

Starting from the first peak, Slavko can choose to go to the first valley, so Slavko wins.

Starting from the second peak, Slavko can choose to go to the second valley, after which Mirko wins
by choosing to go to the fourth peak.

Starting from the third peak, there are no trails, so Mirko wins.

Starting from the fourth peak, Slavko must choose to go to the second valley, after which Mirko wins
by choosing the second peak.

