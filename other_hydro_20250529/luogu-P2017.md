## 题目描述
The cows have taken to racing each other around the farm but they get very dizzy when running in circles, and everyone knows that dizzy cows don't produce any milk. Farmer John wants to convert all of the two-way cow paths in the farm to one-way paths in order to eliminate any 'cycles' and prevent the cows from getting dizzy.  A 'cycle' enables a cow to traverse one or more cow paths and arrive back at her starting point, thus completing a loop or circle.

The farm comprises N pastures (1 <= N <= 100,000) conveniently numbered 1..N. M1 (1 <= M1 <= 100,000) one-way cow paths and M2 two-way cow paths (1 <= M2 <= 100,000) connect the pastures. No path directly connects a pasture to itself, although multiple paths might connect two different pastures. A cow may or may not be able to travel between any two given pastures by following a sequence of cow paths.

Your job is to assign a direction to the two-way cow paths such that the entire farm (ultimately with only one-way paths) has no cycles. That is, there should be no sequence of one-way cow paths which leads back to its starting position. The existing one-way cow paths do not form a cycle and should be left as they are.

One-way cow paths run from pasture A\_i (1 <= A\_i <= N) to pasture B\_i (1 <= B\_i <= N). Two-way cow paths connect pastures X\_i (1 <= X\_i <= N) and Y\_i (1 <= Y\_i <= N).

Consider this example:

```cpp
1-->2 
|  /| 
| / | 
|/  | 
3<--4 
```
The cow paths between pastures 1 and 3, 2 and 3, and 2 and 4 are two-way paths. One-way paths connect 1 to 2 and also 4 to 3. One valid way to convert the two-way paths into one-way paths in such a way that there are no cycles would be to direct them from 1 to 3, from 2 to 3, and from 3 to 4:

```cpp
1-->2 
|  /| 
| / | 
vL  v 
3<--4 
```


## 输入格式
第一行三个整数 $n,m_1,m_2$，分别表示点数，有向边的数量，无向边的数量。

第二行起输入 $m_1$ 行，每行 $2$ 个整数 $a,b$，表示 $a$ 到 $b$ 有一条有向边。

接下来输入 $m_2$ 行，每行 $2$ 个整数 $a,b$，表示 $a$ 和 $b$ 中间有一条无向边。


## 输出格式
对于每条无向边，我们要求按输入顺序输出你定向的结果，也就是如果你输出 $a\ b$，那表示你将 $a$ 和 $b$ 中间的无向边定向为 $a \to b$。

注意，也许存在很多可行的解。你只要输出其中任意一个就好。


## 题目大意
奶牛们发现，在农场里面赛跑是很有趣的一件事.可是她们一旦在农场里面不断地转圈，就 会变得头晕目眩.众所周知，眩晕的奶牛是无法产奶的.于是，农夫约翰想要把他农场里面的双 向道路全部改为单向道路，使得他的农场里面一个圈都没有，以避免他的奶牛们被搞得晕头转 向.如果奶牛可以经过若干条道路回到起点，那么这些道路就称为一个圈.

农场有 $n\ (1 < n < 100000)$ 片草地，编号为 $1$ 到 $n$。这些草地由 $m_1$ 条单向 道路和 $m_2$ 条双向道路连接起来.任何一条道路都不会把一片草地和这片草地本身连接起来.但是，任意两片草地之间都可能有多条道路连接.不保证任意两片草地之间都有路 径相连。

你的任务是给所有的双向道路设定一个方向，使得整个农场(只剩下单向道路)最后一个圈都没有。也就是说，不存在一个单向道路序列的终点和起点重合。数据保证一开始就有的单向道路中，一个圈都没有。而且一开始就有的单向道路不能改变。

单向道路的起点是草地 $A_i$，终点是草地 $B_i$。双向道路连接草地 $X_i,Y_i$。


```input1
4 2 3
1 2
4 3
1 3
4 2
3 2

```

```output1
1 3
4 2
2 3
```

