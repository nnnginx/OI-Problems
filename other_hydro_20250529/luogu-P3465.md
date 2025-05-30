## 题目描述
King Byteasar has yielded under pressure of Byteotian merchants and  hence decided to settle the issue of toll paid by them.

Byteotia consists of $n$ towns connected with $m$ bidirectional roads.

Each road connects directly two different towns and no two towns are  connected by more than one direct road.

Note that the roads may lead through tunnels or flyovers.

Until now each town in Byteotia imposed duty on everyone who  either entered or left the town.

The merchants, discontented with such situation, lodged a protest  against multiple taxation.

King Byteasar ruled that the town privileges are now restricted.

According to the new royal edict, each town can only charge toll on  merchants travelling by exact one road leading into the town,  regardless of the direction they are travelling in.

Furthermore, for each road, those who travel it cannot be made to pay  the duty to both towns the road connects.

It remains to determine which town should collect toll from which road.

Solving this problem His Highness has commissioned to you.

## Task

Write a programme that:

- reads the Byteotian road system's description from the standard input,

- for each town determines on which road it should impose toll, or claims it is impossible,

- writes out the result to the standard output.


## 输入格式
There are two integers in the first line of the standard input: $n$ and $m$ ($1 \le n \le 100\ 000$, $1 \le n \le 200\ 000$), denoting the number of towns and roads in Byteotia, respectively. The towns are numbered from $1$ to $n$. In next $m$ lines descriptions of the roads follow. In line No. $i$ there are two integers $a_i$ and $b_i$ () meaning that towns $a_i$ and $b_i$ are directly connected by a road.


## 输出格式
If collecting the toll in accordance with the royal edict is impossible, your programme should write the word NIE ('no' in Polish) in the first and only line of the standard output. Otherwise, it should write the word TAK ('yes' in Polish) in the first line, while in the following $n$ lines should tell which city collects toll from which road. Line no. $(i+1)$ should tell on which road the town no. $i$ imposes toll. Since town no. $i$ is obviously one endpoint of this road, it is enough to tell what is the other endpoint. Thus if the town no. $i$ imposes toll on the road connecting it with the town no.$j$ , the line no. $(i+1)$ should contain the number $j$. If more than one solution exists, write out one chosen arbitrarily.


## 题目大意
### 题目描述

给你 $n$ 个点和 $m$ 条双向边，问能否将其中的一些边改成有向边，使得只考虑有向边的情况下每个点的入度都为 $1$ 。

### 输入格式

第一行输入 $n,m(1≤n≤100000,1≤m≤200000)$ ，接下来 $m$ 行每行两个数 $a,b$ 表示点 $a$ 和点 $b$ 之间有一条双向边。输入保证没有重边与自环。

### 输出格式

若没有合法方案，输出 $\verb!NIE!$，否则先在第一行输出 $\verb!TAK!$，然后在第 $i+1$ 行输出点 $i$ 的入度是由哪个点出发的边所得到的。

感谢@hdxrie 提供的翻译。

```input1
4 5
1 2
2 3
1 3
3 4
1 4
```

```output1
TAK
3
3
4
1
```

```input2
4 3
1 3
3 4
2 3
```

```output2
NIE
```

## 提示
样例1：


 ![](https://cdn.luogu.com.cn/upload/pic/6984.png) 

样例2：

![](https://cdn.luogu.com.cn/upload/pic/6985.png)


