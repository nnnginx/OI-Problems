## 题目描述
In a village called Byteville, there are $n$ houses connected with $n-1$ roads.

For each pair of houses, there is a unique way to get from one to another.

The houses are numbered from 1 to $n$.

The house no. 1 belongs to the village administrator Byteasar.

As part of enabling modern technologies for rural areas framework, $n$ computers have been delivered    to Byteasar's house.

Every house is to be supplied with a computer, and it is Byteasar's task to distribute them.

The citizens of Byteville have already agreed to play the most recent version of FarmCraft (the game) as soon as they have their computers.

Byteasar has loaded all the computers on his pickup truck and is about to set out to deliver the goods.

He has just the right amount of gasoline to drive each road twice.

In each house, Byteasar leaves one computer, and immediately continues on his route.

In each house, as soon as house dwellers get their computer, they turn it on and install FarmCraft.

The time it takes to install and set up the game very much depends on one's tech savviness, which is fortunately known for each household.

After he delivers all the computers, Byteasar will come back to his house and install the game on his computer.

The travel time along each road linking two houses is exactly 1 minute, and (due to citizens' eagerness to play) the time to unload a computer is negligible.

Help Byteasar in determining a delivery order that allows all Byteville's citizens    (including Byteasar) to start playing together as soon as possible.

In other words, find an order that minimizes the time when everyone has FarmCraft installed.

## 输入格式
The first line of the standard input contains a single integer $n$($2\le n\le 500\ 000$) that gives the number of houses in Byteville.

The second line contains $n$ integers $c_1,c_2,\cdots,c_n$ ($1\le c_i\le 10^9$),separated by single spaces; $c_i$ is the installation time (in minutes) for the dwellers of house no. i.

The next $n-1$ lines specify the roads linking the houses.

Each such line contains two positive integers $a$ and $b$ ($1\le a<b\le n$), separated by a single space.These indicate that there is a direct road between the houses no. $a$ and $b$.


## 输出格式
The first and only line of the standard output should contain a single integer:

the (minimum) number of minutes after which all citizens will be able to play FarmCraft together.


## 题目大意

### 题目描述

在一个叫做比特村的小村庄中，有 $n-1$ 条路连接着这个村庄中的全部 $n$ 个房子。

每两个房子之间都有一条唯一的通路。这些房子的编号为 $1$ 至 $n$。

$1$ 号房子属于村庄的管理员比特安萨尔。

为了提升村庄的科技使用水平，$n$ 台电脑被快递到了比特安萨尔的房子。每个房子都应该有一台电脑，且分发电脑的任务就落在了比特安萨尔的肩上。

比特村的居民一致同意去玩农场物语这个游戏的最新快照版，而且好消息是他们很快就要得到他们最新的高配置电脑了。

比特安萨尔将所有电脑都装在了他的卡车上，而且他准备好完成这个艰巨的任务了。

**他的汽油恰好够走每条路两遍。**

在每个房子边，比特安萨尔把电脑贴心的配送给居民，且立即前往下一个房子。（配送过程不花费任何时间）

只要每间房子的居民拿到了他们的新电脑，它们就会立即开始安装农场物语。安装农场物语所用的时间根据居民的科技素养而定。幸运的是，每间房子中居民的科技素养都是已知的。

在比特安萨尔配送完所有电脑后，他会回到他自己的 $1$ 号房子去安装他自己的农场物语。

用卡车开过每条路的时间恰好是 $1$ 分钟，而居民开电脑箱的时间可以忽略不计。（因为他们太想玩农场物语了）

请你帮助比特安萨尔算出从开始配送到所有居民都玩上了农场物语的最少时间。

### 输入格式

第一行包含一个整数 $n(2 \leq n \leq 5\times 10^5)$，代表比特村中有多少房子。

第二行包含 $n$ 个整数 $c_1, c_2, ⋯, c_n(1 \leq c_i \leq 10^9)$，每个数都被单个空格隔开。$c_i$ 是第 $i$ 号房间中居民安装农场物语所用的时间。

接下来的 $n-1$ 行代表了每一条路的两个顶点。两个顶点 $a$ 和 $b$ 满足 $1 \leq a < b \leq n$，两个数之间有一个空格。

### 输出格式

一行，包含一个整数，代表题目中所说的最小时间。

感谢@deadpool123 提供的翻译

```input1
6
1 8 9 6 3 2
1 3
2 3
3 4
4 5
4 6

```

```output1
11

```

## 提示
 ![](https://cdn.luogu.com.cn/upload/pic/6971.png) 

给一棵树，走过每条边需要花费一个时间，安装软件又需要花费一个时间，需要遍历整棵树并回到起点，想让所有点中到达时间+安装时间的最大值最小，问这个值是多少


