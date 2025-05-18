## 题目描述
Farmer John's $N$ cows ($1 \leq N \leq 1000$) want to organize an emergency "moo-cast" system for broadcasting important messages among themselves.

Instead of mooing at each-other over long distances, the cows decide to equip themselves with walkie-talkies, one for each cow. These walkie-talkies each have a limited transmission radius, but cows can relay messages to one-another along a path consisting of several hops, so it is not necessary for every cow to be able to transmit directly to every other cow.

The cows need to decide how much money to spend on their walkie-talkies. If they spend $X$, they will each get a walkie-talkie capable of transmitting up to a distance of $\sqrt{X}$. That is, the squared distance between two cows must be at most $X$ for them to be able to communicate.

Please help the cows determine the minimum integer value of $X$ such that a broadcast from any cow will ultimately be able to reach every other cow.


## 输入格式
The first line of input contains $N$.

The next $N$ lines each contain the $x$ and $y$ coordinates of a single cow. These are both integers in the range $0 \ldots 25,000$.


## 输出格式
Write a single line of output containing the integer $X$ giving the minimum amount the cows must spend on walkie-talkies.


## 题目大意
### 题目描述

Farmer John 的 $N$ 头奶牛（$1 \leq N \leq 1000$）希望组织一个紧急的“哞播”系统，用于在它们之间广播重要消息。

为了避免在长距离上互相哞叫，奶牛们决定为自己配备对讲机，每头奶牛一个。这些对讲机每个都有一个有限的传输半径，但奶牛们可以通过多次跳跃的路径中继消息，因此并非每头奶牛都需要能够直接与其他每头奶牛通信。

奶牛们需要决定在对讲机上花费多少钱。如果它们花费 $X$，每头奶牛将获得一个能够传输到 $\sqrt{X}$ 距离的对讲机。也就是说，两头奶牛之间的平方距离必须不超过 $X$，它们才能通信。

请帮助奶牛们确定 $X$ 的最小整数值，使得从任何一头奶牛发出的广播最终能够到达其他所有奶牛。

### 输入格式

输入的第一行包含 $N$。

接下来的 $N$ 行每行包含一头奶牛的 $x$ 和 $y$ 坐标。这些坐标都是 $0 \ldots 25,000$ 范围内的整数。

### 输出格式

输出一行，包含整数 $X$，表示奶牛们在对讲机上必须花费的最小金额。

```input1
4
1 3
5 4
7 2
6 1
```

```output1
17

```

## 提示
感谢@MrMorning 提供翻译


