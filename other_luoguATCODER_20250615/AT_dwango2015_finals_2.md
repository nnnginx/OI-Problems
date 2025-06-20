# AT_dwango2015_finals_2 コメント

## 题目描述

### 题目背景

ニワンゴ君正在考虑动画网站弹幕显示方法的新方案。


在有 $N$ 条评论的视频中，评论将以每秒显示 $1$ 个字符的速度从屏幕左侧向右侧流动。在这些评论中，可以按照任意顺序每隔 $1$ 秒显示一条评论。换句话说，第 $i$ 条显示的评论将在最初显示的评论基础上向右移动 $i-1$ 个字符的位置。

ニワンゴ君希望创建出一种情况，即“ $N$ 条评论在同一位置的字符均相同”。也就是说对于所有 $i$，存在整数 $X$ 和字符 $Y$，使得第 $i$ 条显示的评论的第 $X-i$ 个字符为字符 $Y$。

## 输入格式

输入将从标准输入中给出。

> $ N $ $ S_1 $ $ S_2 $ : $ S_N $

- 第 $ 1 $ 行包含一个整数 $ N\ (2 \le N \le 200) $，表示评论数量。
- 接下来的 $N$ 行包含评论信息。第 $i$ 行包含一个字符串 $S_i$，表示第 $i$ 条评论。字符串 $S_i$ 仅包含小写字母，长度至少为 $1$。所有评论的总长度不超过 $10^5$。

## 输出格式

如果可以通过适当的显示顺序确定评论的流动顺序，使得至少创建一种“所有 $N$ 条评论在同一位置的字符均相同”的情况，则输出 `YES`；否则输出 `NO`。

## 输入输出样例 #1

### 输入 #1

```
3
abcd
bdac
aca
```

### 输出 #1

```
YES
```

## 输入输出样例 #2

### 输入 #2

```
4
dwango
niconico
niwango
ginza
```

### 输出 #2

```
NO
```