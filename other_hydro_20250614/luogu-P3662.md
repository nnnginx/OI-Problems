## 题目描述
The long road through Farmer John's farm has $N$ crosswalks across it, conveniently numbered $1 \ldots N$ ($1 \leq N \leq 100,000$). To allow cows to cross at these crosswalks, FJ installs electric crossing signals, which light up with a green cow icon when it is ok for the cow to cross, and red otherwise. Unfortunately, a large electrical storm has damaged some of his signals. Given a list of the damaged signals, please compute the minimum number of signals that FJ needs to repair in order for there to exist some contiguous block of at least $K$ working signals.

## 输入格式
The first line of input contains $N$, $K$, and $B$ ($1 \leq B, K \leq N$). The next $B$ lines each describe the ID number of a broken signal.

## 输出格式
Please compute the minimum number of signals that need to be repaired in order for there to be a contiguous block of $K$ working signals somewhere along the road.


## 题目大意
### 题目描述

穿过 Farmer John 农场的长路上有 $N$ 个人行横道，方便地用编号 $1 \ldots N$ 标识（$1 \leq N \leq 100,000$）。为了让奶牛能够通过这些横道过马路，FJ 安装了电子过马路信号灯，当奶牛可以安全过马路时，信号灯会显示绿色的奶牛图标，否则显示红色。不幸的是，一场大雷暴损坏了他的一些信号灯。给定损坏信号灯的列表，请计算 FJ 需要修复的最少信号灯数量，以便存在至少 $K$ 个连续的信号灯正常工作。

### 输入格式

输入的第一行包含 $N$、$K$ 和 $B$（$1 \leq B, K \leq N$）。接下来的 $B$ 行每行描述一个损坏信号灯的 ID 编号。

### 输出格式

请计算需要修复的最少信号灯数量，以便在道路上某处存在一个长度为 $K$ 的连续正常工作信号灯块。

```input1
10 6 5
2
10
1
5
9
```

```output1
1
```

