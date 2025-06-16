## 题目描述
Why did the cow cross the road? We may never know the full reason, but it is certain that Farmer John's cows do end up crossing the road quite frequently. In fact, they end up crossing the road so often that they often bump into each-other when their paths cross, a situation Farmer John would like to remedy.

Farmer John raises $N$ breeds of cows ($1 \leq N \leq 100,000$), and each of his fields is dedicated to grazing for one specific breed; for example, a field dedicated to breed 12 can only be used for cows of breed 12 and not of any other breed. A long road runs through his farm. There is a sequence of $N$ fields on one side of the road (one for each breed), and a sequence of $N$ fields on the other side of the road (also one for each breed). When a cow crosses the road, she therefore crosses between the two fields designated for her specific breed.


Had Farmer John planned more carefully, he would have ordered the fields by breed the same way on both sides of the road, so the two fields for each breed would be directly across the road from each-other. This would have allowed cows to cross the road without any cows from different breeds bumping into one-another. Alas, the orderings on both sides of the road might be different, so Farmer John observes that there might be pairs of breeds that cross. A pair of different breeds $(a,b)$ is "crossing" if any path across the road for breed $a$ must intersect any path across the road for breed $b$.


Farmer John would like to minimize the number of crossing pairs of breeds. For logistical reasons, he figures he can move cows around on one side of the road so the fields on that side undergo a "cyclic shift". That is, for some $0 \leq k < N$, every cow re-locates to the field $k$ fields ahead of it, with the cows in the last $k$ fields moving so they now populate the first $k$ fields. For example, if the fields on one side of the road start out ordered by breed as 3, 7, 1, 2, 5, 4, 6 and undergo a cyclic shift by $k=2$, the new order will be 4, 6, 3, 7, 1, 2, 5. Please determine the minimum possible number of crossing pairs of breeds that can exist after an appropriate cyclic shift of the fields on one side of the road.


## 输入格式
The first line of input contains $N$. The next $N$ lines describe the order, by breed ID, of fields on one side of the road; each breed ID is an integer in the range $1 \ldots N$. The last $N$ lines describe the order, by breed ID, of the fields on the other side of the road.


## 输出格式
Please output the minimum number of crossing pairs of breeds after a cyclic shift of the fields on one side of the road (either side can be shifted).


## 题目大意
### 题目描述

为什么奶牛要过马路？我们可能永远无法知道完整的原因，但可以肯定的是，Farmer John 的奶牛确实经常过马路。事实上，它们过马路的频率如此之高，以至于它们的路径交叉时经常会撞到彼此，这种情况 Farmer John 希望能够改善。

Farmer John 饲养了 $N$ 种奶牛（$1 \leq N \leq 100,000$），他的每一块田地都专门用于放牧某一种特定的奶牛品种；例如，专门用于品种 12 的田地只能用于品种 12 的奶牛，而不能用于其他品种。一条长长的马路贯穿他的农场。马路的一侧有一系列 $N$ 块田地（每块田地对应一种品种），马路的另一侧也有一系列 $N$ 块田地（同样每块田地对应一种品种）。当一头奶牛过马路时，它会在为其特定品种指定的两块田地之间穿行。

如果 Farmer John 当初计划得更仔细，他可能会在马路两侧按相同的品种顺序排列田地，这样每块品种的田地就会直接相对。这将使奶牛过马路时，不同品种的奶牛不会撞到彼此。然而，马路两侧的田地顺序可能不同，因此 Farmer John 观察到可能存在一些品种对会交叉。一对不同的品种 $(a,b)$ 是“交叉的”，如果品种 $a$ 的任何过马路路径都必须与品种 $b$ 的任何过马路路径相交。

Farmer John 希望最小化交叉品种对的数量。出于物流原因，他决定可以通过对马路一侧的田地进行“循环移位”来重新安排奶牛的位置。也就是说，对于某个 $0 \leq k < N$，每头奶牛都会移动到其前方 $k$ 块田地，最后 $k$ 块田地的奶牛会移动到前 $k$ 块田地。例如，如果马路一侧的田地最初按品种顺序为 3, 7, 1, 2, 5, 4, 6，并进行 $k=2$ 的循环移位，新的顺序将为 4, 6, 3, 7, 1, 2, 5。请确定在对马路一侧的田地进行适当的循环移位后，可能存在的交叉品种对的最小数量。

### 输入格式

输入的第一行包含 $N$。接下来的 $N$ 行描述了马路一侧田地的品种 ID 顺序；每个品种 ID 是 $1$ 到 $N$ 之间的整数。最后的 $N$ 行描述了马路另一侧田地的品种 ID 顺序。

### 输出格式

请输出在对马路一侧的田地进行循环移位后（可以移位任意一侧），交叉品种对的最小数量。

```input1
5
5
4
1
3
2
1
3
2
5
4
```

```output1
0
```

