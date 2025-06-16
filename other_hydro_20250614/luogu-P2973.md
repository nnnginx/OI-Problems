## 题目描述
The Cows have constructed a randomized stink bomb for the purpose of driving away the Piggies. The Piggy civilization consists of N (2 <= N <= 300) Piggy cities conveniently numbered 1..N connected by M (1 <= M <= 44,850) bidirectional roads specified by their distinct endpoints A\_j and B\_j (1 <= A\_j <= N; 1 <= B\_j <= N). Piggy city 1 is always connected to at least one other city.

The stink bomb is deployed in Piggy city 1. Each hour (including the first one), it has a P/Q (1 <= P <= 1,000,000; 1 <= Q <=

1,000,000; P <= Q) chance of polluting the city it occupies. If it does not go off, it chooses a random road out of the city and follows it until it reaches a new city.  All roads out of a city are equally likely to be chosen.

Because of the random nature of the stink bomb, the Cows are wondering which cities are most likely to be polluted. Given a map of the Piggy civilization and the probability that the stink bomb detonates in a given hour, compute for each city the probability that it will be polluted.

For example, suppose that the Piggie civilization consists of two cities connected together and that the stink bomb, which starts in city 1, has a probability of 1/2 of detonating each time it enters a city:

1--2
We have the following possible paths for the stink bomb (where the last entry is the ending city):

1: 1
2: 1-2
3: 1-2-1

4: 1-2-1-2

5: 1-2-1-2-1

etc.
To find the probability that the stink bomb ends at city 1, we can add up the probabilities of taking the 1st, 3rd, 5th, ... paths above (specifically, every odd-numbered path in the above list). The probability of taking path number k is exactly (1/2)^k - the bomb must not remain in its city for k - 1 turns (each time with a probability of 1 - 1/2 = 1/2) and then land in the last city

(probability 1/2). 

So our probability of ending in city 1 is represented by the sum 1/2 + (1/2)^3 + (1/2)^5 + ... . When we sum these terms infinitely, we will end up with exactly 2/3 as our probability, approximately 0.666666667. This means the probability of landing in city 2 is 1/3, approximately 0.333333333. 

Partial feedback will be provided for your first 50 submissions. 

## 输入格式
\* Line 1: Four space separated integers: N, M, P, and Q

\* Lines 2..M+1: Line i+1 describes a road with two space separated integers: A\_j and B\_j


## 输出格式
\* Lines 1..N: On line i, print the probability that city i will be destroyed as a floating point number. An answer with an absolute error of at most 10^-6 will be accepted (note that you should output at least 6 decimal places for this to take effect).


## 题目大意
奶牛们已经制造了一种随机的臭弹，目的是驱赶小猪们。小猪文明由 $N$（$2 \leq N \leq 300$）个小猪城市构成，这些城市通过 $M$（$1 \leq M \leq 44,850$）条双向道路连接，具体的端点为 $A_j$ 和 $B_j$（$1 \leq A_j \leq N; 1 \leq B_j \leq N$）。小猪城市 1 总是与至少一个其他城市相连。

臭弹在小猪城市 1 部署。每个小时（包括第一个小时），它有 $P/Q$（$1 \leq P \leq 1,000,000; 1 \leq Q \leq 1,000,000; P \leq Q$）的概率污染它所处的城市。如果它没有爆炸，它会随机选择一条离开该城市的道路并沿着这条道路行进，直到到达一个新城市。所有离开一个城市的道路被选择的概率是相等的。

由于臭弹的随机特性，奶牛们想知道哪些城市最有可能被污染。给定小猪文明的地图和臭弹在某一小时内引爆的概率，计算每个城市被污染的概率。

例如，假设小猪文明由两个城市相连，并且臭弹在进入每个城市时都有 $1/2$ 的引爆概率：

$$
1--2
$$

我们有以下臭弹的可能路径（最后一项为结束城市）：

1: 1  
2: 1-2  
3: 1-2-1  
4: 1-2-1-2  
5: 1-2-1-2-1  
等。

要找出臭弹最终在城市 1 的概率，我们可以将上述第 1、3、5... 条路径的概率相加（具体来说，是上面列表中的每条奇数编号路径）。路径编号为 $k$ 的概率恰好为 $(1/2)^k$ —— 弹药在城市中必须停留 $k-1$ 回合（每次概率为 $1 - 1/2 = 1/2$），然后到达最后一个城市（概率为 $1/2$）。

因此我们在城市 1 的概率表示为和：

$$
\frac{1}{2} + \left(\frac{1}{2}\right)^3 + \left(\frac{1}{2}\right)^5 + \ldots
$$

当我们无限地求和这些项时，最终得到的概率正好是 $\frac{2}{3}$，约为 $0.666666667$。这意味着在城市 2 的概率是 $\frac{1}{3}$，约为 $0.333333333$。

```input1
2 1 1 2 
1 2 

```

```output1
0.666666667 
0.333333333 

```

## 提示
感谢 @[Alpha](https://www.luogu.com.cn/user/87058) 贡献 Special Judge。

