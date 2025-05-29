## 题目描述

SJZEZ 和 TSYZ 正在进行一轮足球联谊赛，根据规则，这轮比赛有两场，一场在 SJZEZ 的主场进行，一场在 TSYZ 的主场进行。胜负判断标准如下：

1. 在两场比赛中进球总数较多的一方赢得比赛。
2. 如果双方进球总数相同，在对方主场进球更多的一方赢得比赛。
3. 如果1、2都相同，胜利者将会随机产生。

双方已经进行了一场比赛，作为 SJZEZ 的队长，忘川沧月童鞋想知道：

1. 第二场 sjzez 最少需要进多少球，才有可能赢得比赛。
2. 第二场 sjzez 进不超过多少个球，tsyz 才有可能赢得比赛。

已知在一场比赛中，一方的进球数不可能多于 30 个。

## 输入格式

第一行一个整数 $ t $，表示该测试点中数据的组数。

接下来 $ t $ 行，每行一个字符串，描述该组数据中第一场比赛的情况，形式如下：

```
wccy's team played where game, scored x goals, and conceded y goals.
```

其中 where 是 ```home``` 或者 ```away``` 中的一个，```home``` 表示第一场比赛是在 sjzez 的主场进行，```away``` 表示第一场比赛是在 tsyz 的主场进行。

$ x $ ， $ y $ 是整数，分别表示忘川沧月的队伍的进球数，和对方的进球数。

## 输出格式

输出 $ t $ 行，每行包含两个用空格隔开的整数，分别是两个问题的答案。

## 样例输入

```
2
wccy's team played home game, scored 28 goals, and conceded 0 goals.
wccy's team played home game, scored 1 goals, and conceded 1 goals.
```

## 样例输出

```
0 1
1 29
```

## 数据规模与约定

对于 $100\%$ 的数据，$ 1\leq t\leq 500 $，$ 0\leq x,y\leq 30 $。

## 题目来源

Poetize7

