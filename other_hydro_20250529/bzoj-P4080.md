

## 题目描述
 魔法炮来到了帝都，除了吃特色菜之外，还准备去尝一尝著名的北京烤鸭。帝都一共有 $n(1\le n\le 100)$ 个烤鸭店，可以看成是二维平面内的点。不过由于魔法炮在吃烤鸭之前没有带钱，所以吃完烤鸭之后只能留下刷盘子。刷完盘子之后，魔法炮除了不用付饭费之外，老板还会奖励他 $d(1\le d\le 10000)$ 元钱。魔法炮是一个特么喜欢吃烤鸭的孩子，所以在去过一家烤鸭店之后，魔法炮还准备去其他的烤鸭店。但是由于帝都路费较贵，每单位长度需要花费 $1$ 元钱，所以魔法炮可能去不了所有其他的烤鸭店。在到达下一家烤鸭店之前，魔法炮会花掉手里所有钱，以便于下一次接着吃霸王餐。
 
另外，魔法炮对于自己刷过盘子的烤鸭店有着特殊的感情，所以他要求在某一家烤鸭店吃完烤鸭后，可以到达全部已经吃过去过的烤鸭店。那么问题来了，魔法炮想知道自己最多能去多少家烤鸭店，以及这些烤鸭店都是哪些。你能帮帮他吗？


**题目大意**：给定平面内的 $n$ 个点，选出一个点集 $S$，使得 $S$ 里的所有点两两之间欧几里得距离不超过 $d$，问 $|S|$ 的最大值以及 $S$ 里的点都有哪些。若答案有多种，输出任意一个。
第一行两个整数 $n$ 和 $d$，分别表示烤鸭店数和老板给魔法炮的路费。
## 输入格式
第一行输入两个正整数数 $n$ 和 $d$，分别表示烤鸭店的数量和老板奖励他的价钱。

接下来 $n$ 行，每行两个整数 $x,y$，表示 $n$ 个烤鸭店的坐标。

## 输出格式
第一行一个数 $m$，表示魔法炮最多能去多少家烤鸭店。
第二行 $m$ 个数，每个数表示魔法炮能去的烤鸭店标号。

```input1
4 1
0 0
0 1
1 0
1 1

```

```output1
2
1 2
```

## 提示
 对于 $100\%$ 的数据：$1\le n\le 100$，$1\le d\le 10000$，$-10000\le x,y\le 10000$。
 
## 题目来源
鸣谢ZidaneAndMessi


