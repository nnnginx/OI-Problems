## 题目描述
Farmer John tries to keep the cows sharp by letting them play with intellectual toys. One of the larger toys is the lights in the barn. Each of the $N (2 \le N \le 10^5)$ cow stalls conveniently numbered $1\ldots N$ has a colorful light above it.

At the beginning of the evening, all the lights are off. The cows control the lights with a set of N pushbutton switches that toggle the lights; pushing switch i changes the state of light i from off to on or from on to off.

The cows read and execute a list of $M(1\le M \le 10^5)$ operations expressed as one of two integers ( $0 \le$ operation $\le 1$ ).

The first kind of operation (denoted by a $0$ command) includes two subsequent integers $S_i$ and $E_i (1 \le S_i \le E_i \le N)$ that indicate a starting switch and ending switch. They execute the operation by pushing each pushbutton from $S_i$ through $E_i$ inclusive exactly once.

The second kind of operation (denoted by a $1$ command) asks the cows to count how many lights are on in the range given by two integers $S_i$ and $E_i (1 \le S_i \le E_i \le N)$ which specify the inclusive range in which the cows should count the number of lights that are on.

Help FJ ensure the cows are getting the correct answer by processing the list and producing the proper counts.

农夫约翰试图让奶牛玩智力玩具来保持它们的敏锐。谷仓里的灯是较大的玩具之一。$N (2 \le N \le 10^5)$ 个牛栏编号为 $1 \ldots N$，每个牛栏上面都有一盏灯。起初所有的灯都关着。

共有 $M$ 次操作，分为两种。
1. 指定一个区间 $[S_i,E_i]$，然后改变编号在这个区间内的灯的状态（把开着的灯关上，关着的灯打开）；
2. 指定一个区间 $[S_i,E_i]$，要求你输出这个区间内有多少盏灯是打开的。







## 输入格式
第 $1$ 行: 用空格隔开的两个整数 $N$ 和 $M$，$N$ 是灯数。

第 $2\ldots M+1$ 行: 每行表示一个操作, 有三个用空格分开的整数: 指令号, $S_i$ 和 $E_i$。

若指令号为 $0$，则表示改变 $[S_i,E_i]$ 区间内的灯的状态（把开着的灯关上，关着的灯打开）。

若指令号为 $1$，则表示输出 $[S_i,E_i]$ 这个区间内有多少盏灯是打开的。

```input1
4 5
0 1 2
0 2 4
1 2 3
0 2 4
1 1 4
```

```output1
1
2
```

## 提示
| 数据点编号 | $N$ | $M$ |
| :----------: | :----------: | :----------: |
| $1\sim 2$ | $\le 100$ | $\le 100$ |
| $3\sim 4$ | $\le 1000$ | $\le 1000$ |
| $5\sim 6$ | $\le 10000$ | $\le 10000$ |
| $7\sim 8$ | $\le 10^5$ | $\le 100$ |
| $9\sim 10$ | $\le 100$ | $\le 10^5$ |
| $11\sim 12$ | $\le 1000$ | $\le 10^5$ |
| $13\sim 14$ | $\le 10^5$ | $\le 1000$ |
| $15\sim 16$ | $\le 10000$ | $\le 10000$ |
| $17\sim 18$ | $\le 10$ | $\le 10^5$ |
| $19\sim 20$ | $\le 2000$ | $\le 10^6$ |


