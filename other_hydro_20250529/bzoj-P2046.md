## 题目描述
Hst 是个爱思考的好孩子。这一天 LL 博士给了他一道题目做，如下：
```plain
鼹鼠是一种很喜欢挖洞的动物，但每过一定的时间，它还是喜欢把头探出到地面上来透透气的。根据这个特点阿牛编写了一个打鼹鼠的游戏：在一个 n*n 的网格中，在某些时刻鼹鼠会在某一个网格探出头来透透气。你可以控制一个机器人来打鼹鼠，如果 i 时刻鼹鼠在某个网格中出现，而机器人也处于同一网格的话，那么这个鼹鼠就会被机器人打死。而机器人每一时刻只能够移动一格或停留在原地不动。机器人的移动是指从当前所处的网格移向相邻的网格，即从坐标为（i,j）的网格移向(i-1,j),(i+1,j),(i,j-1),(i,j+1)四个网格，机器人不能走出整个 n*n 的网格。游戏开始时，你可以自由选定机器人的初始位置。现在知道在一段时间内，鼹鼠出现的时间和地点，请编写一个程序使机器人在这一段时间内打死尽可能多的鼹鼠。
【输入格式】（input.txt）
从文件 input.txt 中读入数据，文件第一行为 n（n<=1000）, m（m<=10000），其中 m 表示在这一段时间内出现的鼹鼠的个数，接下来的 m 行中每行有三个数据 time,x,y 表示有一只鼹鼠在游戏开始后 time 个时刻，在第 x 行第 y 个网格里出现了一只鼹鼠。Time 按递增的顺序给出。注意同一时刻可能出现多只鼹鼠，但同一时刻同一地点只可能出现一只鼹鼠。
【输出格式】（output.txt）输出文件 output.txt 中仅包含一个正整数，表示被打死鼹鼠的最大数目。
【输入输出样例】
input.txt output.txt 2 2 1 1 1 1 2 2 2
```
这不是我们的问题，当然这道题相信大家都知道是出自 HNOI2004 的第一题：打鼹鼠。Hst 可是很聪明的哟，他花了 $0.5$ 分钟就想出来怎么做并且编完了。但是他又提出了一个新的问题：有 $m$ 只鼹鼠出现在一个 $1\sim n$ 的长条上。对于第 $k$ 只鼹鼠，我们用 $t_k,w_k,x_k$ 来描述。即在 $t_k$ 时刻，会有一只分值为 $w_k$ 的鼹鼠 $k$ 出现在位置 $x_k$ 上。现在你有一个锤头，每一时刻它都停留在一个位置上。你可以用它不费时间的敲死一只鼹鼠并得到相应的分值。但是每个时刻你的锤头最多只能移动 $p$ 格。也就是说如果 $s$ 时刻你在位置 $pos$，那么 $s+1$ 时刻你运动到位置 $pos–p \sim pos+p$。在零时刻你的锤子可以在任意位置。鼹鼠出现的时刻大于 $0$。同时我们保证同一时间同一位置不会有两只鼹鼠出现，因为他们太胖了。
## 输入格式
第一行两个正整数 $n,m$。然后 $m$ 行每行三个正整数 $t_k,w_k,x_k$ 描述第 $k$ 只鼹鼠。注意，本题输入数据较大，对于使用 C++ 的选手需要使用 `scanf` 来读入。
## 输出格式
只有一行一个整数为最大得分。
## 样例输入
```plain
5 20 1
2 17392 5
3 21061 3
5 21177 4
6 25416 1
7 23512 4
9 27947 1
13 12313 3
14 1126 515 27358 2
16 17741 3
17 23412 4
18 32142 2
19 7729 2
20 23539 1
22 15923 2
26 5083 1
31 6022 1
33 24950 3
34 29713 2
35 13623 5
```
## 样例输出
```plain
276937
```
## 数据规模与约定
对于 $100\%$ 的数据，$n\times m\leq 10^{12}$，$pn\leq10^5$，$m\leq10^5$，$0\leq p\leq5$，$t_k\leq 10^6$。
## 题目来源
第一届「NOIer」全国竞赛