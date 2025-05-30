## 题目描述

为了得到书法大家的真传，小 E 同学下定决心去拜访住在魔法森林中的隐士。

魔法森林可以被看成一个包含 $N$ 个节点 $M$ 条边的无向图，节点标号为 $1,\ldots,N$，边标号为 $1,\ldots,M$。初始时小 E 同学在号节点 $1$，隐士则住在 $N$ 号节点。小 E 需要通过这一片魔法森林，才能够拜访到隐士。

魔法森林中居住了一些妖怪。每当有人经过一条边的时候，这条边上的妖怪就会对其发起攻击。幸运的是，在 $1$ 号节点住着两种守护精灵：$A$ 型守护精灵与 $B$ 型守护精灵。小 E 可以借助它们的力量，达到自己的目的。

只要小 E 带上足够多的守护精灵，妖怪们就不会发起攻击了。具体来说，无向图中的每一条边 $E_i$ 包含两个权值 $A_i$ 与 $B_i$。若身上携带的 A 型守护精灵个数不少于 $A_i$，且 $B$ 型守护精灵个数不少于 $B_i$，这条边上的妖怪就不会对通过这条边的人发起攻击。当且仅当通过这片魔法森林的过程中没有任意一条边的妖怪向小 E 发起攻击，他才能成功找到隐士。

由于携带守护精灵是一件非常麻烦的事，小 E 想要知道，要能够成功拜访到隐士，最少需要携带守护精灵的总个数。守护精灵的总个数为 $A$ 型守护精灵的个数与 $B$ 型守护精灵的个数之和。

## 输入格式

第一行包含两个整数 $N,M$，表示无向图共有 $N$ 个节点，$M$ 条边。  
接下来 $M$ 行，第 $i$ 行包含四个正整数 $X_i,Y_i,A_i,B_i$，描述第 $i$ 条无向边。其中 $X_i$ 与 $Y_i$ 为该边两个端点的标号，$A_i$ 与 $B_i$ 的含义如题所述。 

**注意**：数据中可能包含重边与自环。

## 输出格式

输出一行一个整数：如果小 E 可以成功拜访到隐士，输出小 E 最少需要携带的守护精灵的总个数；  
如果无论如何小 E 都无法拜访到隐士，输出 “``-1``”（不含引号）。

```input1
4 5
1 2 19 1
2 3 8 12
2 4 12 15
1 3 17 8
3 4 1 17
```

```output1
32
```

```input2
3 1
1 2 1 1
```

```output2
-1
```

## 数据范围与提示

对所有的数据，$2 \leq n \leq 50000,\ 0 \leq m \leq 100000,\ 1 \leq a_i ,b_i \leq 50000$。

