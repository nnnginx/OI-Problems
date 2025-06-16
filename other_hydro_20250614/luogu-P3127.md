## 题目描述
Farmer John has received a shipment of N large hay bales ($1 \le N \le 100,000$), and placed them at various locations along the road leading to his barn. Unfortunately, he completely forgets that Bessie the cow is out grazing along the road, and she may now be trapped within the bales! Each bale $j$ has a size $S_j$ and a position $P_j$ giving its location along the one-dimensional road.  Bessie the cow can move around freely along the road, even up to the position at which a bale is located, but she cannot cross through this position.  As an exception, if she runs in the same direction for $D$ units of distance, she builds up enough speed to break through and permanently eliminate any hay bale of size strictly less than $D$.  Of course, after doing this, she might open up more space to allow her to make a run at other hay bales, eliminating them as well.

Bessie can escape to freedom if she can eventually break through either the  leftmost or rightmost hay bale.  Please compute the total area of the road consisting of real-valued starting positions from which Bessie cannot escape.



## 输入格式
The first line of input contains $N$.  Each of the next $N$ lines describes a bale, and contains two integers giving its size and position, each in the range $1\ldots 10^9$. All positions are distinct.


## 输出格式
Print a single integer, giving the area of the road from which Bessie cannot escape.

## 题目大意
### 题目描述

Farmer John 收到了一批 $N$ 个大型干草捆（$1 \le N \le 100,000$），并将它们放置在他通往谷仓的道路上的不同位置。不幸的是，他完全忘记了奶牛 Bessie 正在这条路上吃草，她现在可能被困在这些干草捆之间了！每个干草捆 $j$ 有一个大小 $S_j$ 和一个位置 $P_j$，表示它在这条一维道路上的位置。Bessie 可以在道路上自由移动，甚至可以移动到干草捆所在的位置，但她无法穿过这个位置。唯一的例外是，如果她朝同一方向连续移动 $D$ 单位的距离，她将获得足够的速度，能够突破并永久消除任何大小严格小于 $D$ 的干草捆。当然，在突破之后，她可能会打开更多的空间，从而有机会突破其他干草捆，并继续消除它们。

如果 Bessie 最终能够突破最左侧或最右侧的干草捆，她就可以成功逃脱。请计算道路中所有无法逃脱的实数起始位置的总面积。

### 输入格式

输入的第一行包含 $N$。接下来的 $N$ 行描述每个干草捆，每行包含两个整数，分别表示干草捆的大小和位置，范围均为 $1 \ldots 10^9$。所有位置均不相同。

### 输出格式

输出一个整数，表示 Bessie 无法逃脱的道路总面积。

```input1
5
8 1
1 4
8 8
7 15
4 20
```

```output1
14
```

