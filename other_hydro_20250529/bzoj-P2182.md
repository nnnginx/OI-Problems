

## 题目描述

Jiajia is the king of the GbAaY Kingdom. He always squeezes his 20 ministers as coolies. There are $n$ cities and $m$ two-way roads connecting cities in the kingdom. Because of the increasing of the oil fee, he want to simplify the road system in the GbAaY Kingdom to save the traffic cost.

Thus, some of roads will be removed. But he requests the ministers guarantee that there is always a path between any two cities. GbAaY Minister Loner suggests Jiajia for the convenience of the traffic management, the farthest distance between cities should be minimal. Unhesitatingly, Jiajia agrees this resolution. As the GbAaY Kingdom's minister (cooly), you must work hard for Jiajia to make the simplification plan.

JiaJia 是 GbAaY 王国的王（高贵ing……） 他每天都要挤出 20 分钟用在做菜上面。 他的王国有 $n$ 个城市，由 $m$ 条双向边所连接着。 因为石油的价格上涨，他想把 GbAaY 王国的交通简化，好节约交通花费。

于是，有些路径需要被移除，但是依然保证移除之后依然有路径连接任意两个城市。

GbAaY 的大臣 Loner 建议 JiaJia，为了使交通管理的方便， 整个城市中最长的一条路径需要他的值最小。

JiaJia 迅速答应了大臣的这个决定。你作为 GbAaY 王国的一个大臣，你必须帮助 JiaJia 简化这个问题 

## 输入格式

The first line contains two integers $n, m$ .

Each line of the following $m$ lines contains three integers $u, v, w$ . They denote there is a road with length $w$ between city $u$ and city $v$ .

第一行有两个正整数 $n,m$。

接着 $m$ 行每行三个正整数 $u,v,w$，描述一条连接 $u,v$ 的双向边的长度是 $w$。

## 输出格式

The first line contains one integer which is the farthest distance between cities after the simplification. 

输出第一行有一个正整数表示在简化交通后最远的两个城市的距离。 

## 样例输入

```plain
3 3
1 2 1
2 3 1
1 3 1
```

## 样例输出

```plain
2
```

## 数据规模与约定

对于 $100\%$ 的数据，保证：$1 \leq n \leq 200$，$n - 1 \leq m \leq 5\times 10^4$，$u \neq v, 0 \leq w \leq 10^5$。