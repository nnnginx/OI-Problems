## 题目描述
The layout of Farmer John's farm is quite peculiar, with a large circular road running around the perimeter of the main field on which his cows graze during the day. Every morning, the cows cross this road on their way towards the field, and every evening they all cross again as they leave the field and return to the barn.

As we know, cows are creatures of habit, and they each cross the road the same way every day. Each cow crosses into the field at a different point from where she crosses out of the field, and all of these crossing points are distinct from each-other. Farmer John owns $N$ cows, conveniently identified with the integer IDs $1 \ldots N$, so there are precisely $2N$ crossing points around the road. Farmer John records these crossing points concisely by scanning around the circle clockwise, writing down the ID of the cow for each crossing point, ultimately forming a sequence with $2N$ numbers in which each number appears exactly twice. He does not record which crossing points are entry points and which are exit points.

Looking at his map of crossing points, Farmer John is curious how many times various pairs of cows might cross paths during the day. He calls a pair of cows $(a,b)$ a "crossing" pair if cow $a$'s path from entry to exit must cross cow $b$'s path from entry to exit. Please help Farmer John count the total number of crossing pairs.

## 输入格式
The first line of input contains $N$ ($1 \leq N \leq 50,000$), and the next $2N$ lines describe the cow IDs for the sequence of entry and exit points around the field.


## 输出格式
Please print the total number of crossing pairs.


## 题目大意
### 题目描述

Farmer John 的农场布局非常独特，主田地的外围有一条环形道路，他的奶牛白天在这里吃草。每天早上，奶牛们都会穿过这条道路进入田地，每天晚上它们又会再次穿过这条道路离开田地返回牛棚。

众所周知，奶牛是习惯性动物，它们每天都会以相同的方式穿过道路。每头奶牛进入田地的点和离开田地的点不同，并且所有这些穿过点都彼此不同。Farmer John 拥有 $N$ 头奶牛，方便地用整数 ID $1 \ldots N$ 标识，因此道路周围恰好有 $2N$ 个穿过点。Farmer John 通过顺时针扫描环形道路，记录每个穿过点的奶牛 ID，最终形成一个包含 $2N$ 个数字的序列，其中每个数字恰好出现两次。他并未记录哪些穿过点是进入点，哪些是离开点。

看着他的穿过点地图，Farmer John 好奇一天中不同奶牛对之间可能会交叉多少次。如果奶牛 $a$ 从进入点到离开点的路径必须与奶牛 $b$ 从进入点到离开点的路径交叉，那么他称奶牛对 $(a,b)$ 为“交叉”对。请帮助 Farmer John 计算交叉对的总数。

### 输入格式

输入的第一行包含 $N$ ($1 \leq N \leq 50,000$)，接下来的 $2N$ 行描述了田地周围进入和离开点的奶牛 ID 序列。

### 输出格式

请输出交叉对的总数。

```input1
4
3
2
4
4
1
3
2
1
```

```output1
3
```

