# AT_dwango2015_finals_4 コインの取り合い

## 题目描述

## 题面描述

尼旺戈和尼科莫巴在玩一种硬币游戏。

开始 $ N $ 个硬币排列在 $ 1 $ 行，硬币上从左到右依次有 $ 1 $ 到 $ N $ 的编号。奇数号的硬币正面朝上，偶数号的硬币背面朝上。第 $ i $ 枚硬币的价值是 $ S_i $ 。

这个游戏由 $ N - 1 $ 回合组成，奇数回合的玩家是尼旺戈，偶数回合的玩家是尼科莫巴。在第 $ i $ 回合中，玩家有三种操作：

- 翻编号为 $ i $ 的硬币
- 翻编号为 $ i + 1 $ 的硬币
- 不做任何操作

$ N - 1 $ 回合结束后，尼旺戈获得面朝上的硬币，尼科莫巴获得背面的硬币。此时，自己获得的硬币价值之和将成为玩家的得分。但是，因为两个人都很聪明，所以每个人都会采取将自己的分数最大化的最佳战略。

另外，在开始游戏之前，尼科莫巴会在硬币上涂鸦，硬币的价值会下降。尼古莫巴共涂鸦 $ Q $ 次，第 $ i $ 次涂鸦的硬币是硬币 $ P_i $，因为涂鸦，硬币 $ i $ 的价值下降了$ D_i $ 。

关于 $ Q $ 次的涂鸦，请计算在给硬币涂鸦之后开始游戏时尼旺戈的得分。

## 输入格式

输入参见以下格式：

```
 $ N $ 
 $ S_1 $   $ S_2 $  ...  $ S_N $ 
 $ Q $ 
 $ P_1 $   $ D_1 $ 
 $ P_2 $   $ D_2 $ 
:
 $ P_Q $   $ D_Q $ 
```

## 输出格式

输出由 $ Q + 1 $ 行构成。在第 $ 1 $ 行中，输出从开始的状态开始游戏时的尼旺戈的得分，在从第 $ 2 $ 行到 $ Q + 1 $ 行中的第 $ i $ 行中，输出在第 $ i $ 次涂鸦之后开始游戏时的尼旺戈君的得分。在输出的末尾要加换行。

## 输入输出样例 #1

### 输入 #1

```
4
1 2 3 4
1
4 3
```

### 输出 #1

```
7
5
```

## 输入输出样例 #2

### 输入 #2

```
8
3 1 4 1 5 9 2 6
5
3 3
6 6
8 4
1 1
6 2
```

### 输出 #2

```
19
16
16
12
11
11
```