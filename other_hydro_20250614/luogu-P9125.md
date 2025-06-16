## 题目描述
**Note: The time limit for this problem is 4s, two times the default.**

Somebody has been grazing in Farmer John's $G(1 \le G \le 10^5)$ private gardens! Using his expert forensic knowledge, FJ has been able to determine the precise time each garden was grazed. He has also determined that there was a single cow that was responsible for every grazing incident. 

In response to these crimes each of FJ's $N(1 \le N \le 10^5)$ cows have provided an alibi that proves the cow was in a specific location at a specific time. Help FJ test whether each of these alibis demonstrates the cow's innocence. 

A cow can be determined to be innocent if it is impossible for her to have travelled between all of the grazings and her alibi. Cows travel at a rate of $1$ unit distance per unit time. 

## 输入格式
The first line of input will contain $G$ and $N$ separated by a space.

The next $G$ lines contain the integers $x, y$, and $t (−10^9 \le x,y \le 10^9;0 \le t \le 10^9)$

separated by a space describing the location and time of the grazing. It will always be possible for a single cow to travel between all grazings.

The next $N$ lines contain $x$, $y$, and $t(−10^9 \le x,y \le 10^9;0 \le t \le 10^9)$ separated by a space describing the location and time of each cow's alibi. 

## 输出格式
Output a single integer: the number of cows with alibis that prove their innocence. 

## 题目大意
### 题目描述

注意：本题的时间限制为 4 秒，是默认限制的两倍。

有人在 Farmer John 的 $G(1 \leq G \leq 10^5)$ 个私人花园里偷吃了庄稼！通过他的专业法医知识，Farmer John 确定了每个花园被偷吃的具体时间。他还发现，这些事件的罪魁祸首是一头单独的奶牛。

为了回应这些犯罪行为，Farmer John 的 $N(1 \leq N \leq 10^5)$ 头奶牛每头都提供了一个不在作案现场的证明（即“不在场证明”），表明奶牛在特定时间出现在特定位置。请帮助 Farmer John 判断这些“不在场证明”中哪些能够证明奶牛的清白。

如果一头奶牛无法在她的“不在场证明”位置与所有被偷吃地点之间往返，则可以确定这头奶牛是清白的。奶牛的移动速度为每单位时间 $1$ 单位距离。本题中提到的距离均为欧几里得距离。

### 输入格式

第一行包含两个用空格分隔的整数 $G$ 和 $N$。

接下来的 $G$ 行，每行包含三个用空格分隔的整数 $x, y, t$（$-10^9 \leq x, y \leq 10^9; 0 \leq t \leq 10^9$），描述某次偷吃事件的地点和时间。可以保证单独一头奶牛可以在所有被偷吃地点之间往返。

接下来的 $N$ 行，每行包含 $x, y, t$（$-10^9 \leq x, y \leq 10^9; 0 \leq t \leq 10^9$），描述某头奶牛的“不在场证明”中提到的位置和时间。

### 输出格式

输出一个整数，表示能够证明清白的奶牛的数量。

### 样例 1 的解释

共有两次偷吃事件，第一次发生在 $(0,0)$，时间为 $100$；第二次发生在 $(50,0)$，时间为 $200$。

- 第一头奶牛的“不在场证明”无法证明她的清白。她刚好有足够的时间到达第一次偷吃事件的地点。
- 第二头奶牛的“不在场证明”能够证明她的清白。她远离任何偷吃事件的地点。
- 不幸的是，第三头奶牛在偷吃事件的现场，这并不能证明她的清白。
- 最后，第四头奶牛是清白的，因为她不可能在时间限制内从她的“不在场证明”地点赶到最后一次偷吃事件的地点。

### 评分标准

- 测试点 $2-4$：$1 \leq G, N \leq 10^3$。此外，对于偷吃地点和“不在场证明”，$-10^6 \leq x, y \leq 10^6$ 且 $0 \leq t \leq 10^6$。
- 测试点 $5-11$：无额外限制。

```input1
2 4
0 0 100
50 0 200
0 50 50
1000 1000 0
50 0 200
10 0 170
```

```output1
2
```

## 提示
### Explanation for Sample 1

There were two grazings; the first at $(0,0)$ at time 100 and the second at $(50,0)$ at time $200$.

The first cow's alibi does not prove her innocence. She has just enough time to arrive at the first grazing.

The second cow's alibi does prove her innocence. She is nowhere near any of the grazings.

Unfortunately for the third cow, being at the scene of the crime does not prove innocence.

Finally, the fourth cow is innocent because it's impossible to make it from her alibi to the final grazing in time. 

### SCORING

 - Inputs $2-4$: $1 \le G,N \le 10^3$. Also, for both the fields and alibis, $−10^6 \le x,y \le 10^6$ and $0 \le t \le 10^6$.
 - Inputs $5-11$: No additional constraints.

