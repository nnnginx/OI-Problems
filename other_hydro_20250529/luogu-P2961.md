## 题目描述
Farmer John's N (1 <= N <= 1,000) cows conveniently numbered 1..N decided to form M (1 <= M <= 100) study groups. A total of S\_i (1 <= S\_i <= 19) cows study in group G\_i (namely cows G\_i1, G\_i2, ...). A cow might study in more than one study group.

For each study group, one cow in the group must be chosen to bring cookies to the meeting. Cookies are costly and require time to acquire, so the cows want to divide the work of bringing cookies as fairly as possible.

They decided that if a cow attends meetings with size c\_1, c\_2, ..., c\_K, she is only willing to bring cookies to at most ceil(1/c\_1 + 1/c\_2 + ... + 1/c\_K) meetings.

Figure out which cow brings cookies to each meeting. If this isn't possible, just output '-1'. Choose any solution if more than one is possible.



## 输入格式
\* Line 1: Two space-separated integers: N and M

\* Lines 2..M+1: Line i+1 contains many space-separated integers: S\_i, G\_i1, G\_i2, ...


## 输出格式
\* Lines 1..M: If a mapping is possible, line i contains the number of the cow who brings cookies to study group i. Otherwise, line 1 contains just the integer -1.


## 题目大意
农夫约翰的 $N(1 \le N \le 1000)$ 只奶牛（编号为 $1$ 到 $N$）决定成立 $M(1 \le M \le 100)$ 个学习小组。在学习小组 $G_i$ 中有 $S_i$ 只牛，分别为牛$G_{i1},G_{i2},\cdots$，一头牛可能会参加多个小组。

对于每个学习小组，有一只牛必须在每次聚会的时候带饼乾饮料请大家吃（衰～）。因为买这些零食会消耗牛们那为数不多的零花钱，还会花费牛们宝贵的时间，所以牛们希望尽可能公平地分摊带零食的责任。 牛们决定。如果一只牛参加了 $K$ 个学习小组，$K$ 个学习小组的大小分别为 $c_1,c_2, \cdots c_K$，那麽她最多负责为 $\lceil \frac{1}{c_1} + \frac {1}{c_2} + \cdots + \frac{1}{c_K} \rceil$ 个学习小组的聚会带零食。其中 $\lceil \rceil$为上取整函数。 请计算出一个方案，决定每个学习小组的聚会由哪一头牛负责带零食。如果没有一种方案可行，输出 `-1`。


```input1
5 6 
3 2 4 5 
2 1 3 
3 1 2 3 
1 1 
2 2 5 
3 2 3 4 

```

```output1
5 
1 
3 
1 
2 
4 

```

## 提示
Cow1 can bring cookies to at most 2 meetings, cow2 can bring 2, cow3 can bring 2, cow4 can bring 1, and cow5 can bring 1.


