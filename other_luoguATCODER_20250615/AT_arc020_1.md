# AT_arc020_1 [ARC020A] 石を滑らせるゲーム

## 题目描述

蚂蚁Ant和Bug在玩一个关于石头的游戏。这个游戏使用一根笔直的细长的冰板和两个小的石头。冰板每1毫米有1000，-1000两种刻度。开始两只游戏蚂蚁玩家有一块石头。两只蚂蚁游戏者交替地从木板边缘滑动石头。然后，最终滑动的石头更接近0度刻度的玩家将成为该游戏的胜者。此外，如果两个石头上的距离为0，则判为平局。为了Ant先生和Bug先生这两只好玩的蚂蚁，请制定出两个棋子位置的刻度分别被给予时判定胜负的程序。

## 输入格式

--------

1,000≦A≦1,000 -1,000≦B≦1,000

其中A表示ANT，B表示BUG

## 输出格式

--------

若ANT获胜输出“Ant”

若BUG获胜输出“Bug”

若为平局输出“Draw”

## 输入输出样例 #1

### 输入 #1

```
2 3
```

### 输出 #1

```
Ant
```

## 输入输出样例 #2

### 输入 #2

```
1 0
```

### 输出 #2

```
Bug
```

## 输入输出样例 #3

### 输入 #3

```
-100 100
```

### 输出 #3

```
Draw
```