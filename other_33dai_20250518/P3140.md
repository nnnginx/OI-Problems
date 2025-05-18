## 题目描述
After the last debacle involving Farmer John's circular barn, one would think he had learned his lesson about non-traditional architecture.  However, he thinks he can still make his circular barn (from the preceding problem) function properly by allowing multiple cows into each room.  To recap, the barn consists of a ring of $n$ rooms,  numbered clockwise from $1 \ldots n$ around the perimeter of the barn ($3 \leq n \leq 100$).  Each room has doors to its two neighboring rooms, and also a door opening to the exterior of the barn.

Farmer John wants exactly $r_i$ cows to end up in room $i$ ($1 \leq r_i \leq 1,000,000$). To herd the cows into the barn in an orderly fashion, he plans to unlock $k$ exterior doors ($1 \leq k \leq 7$), allowing the cows to enter through only those doors. Each cow then walks clockwise through the rooms until she reaches a suitable destination.  Farmer John wants to unlock the exterior doors that will cause his cows to collectively walk a minimum total amount of distance after entering the barn (they can initially line up however they like outside the $k$ unlocked doors; this does not contribute to the total distance in question).  Please determine the minimum total distance his cows will need to walk, if he chooses the best $k$ such doors to unlock.

## 输入格式
The first line of input contains $n$ and $k$.  Each of the remaining $n$ lines contain $r_1 \ldots r_n$.


## 输出格式
Please write out the minimum amount of distance the cows need to travel.


## 题目大意
### 题目描述

在上一次涉及 Farmer John 的圆形谷仓的惨败之后，人们可能会认为他已经吸取了关于非传统建筑的教训。然而，他认为通过允许每间房间进入多头奶牛，仍然可以让他那个圆形谷仓（来自之前的问题）正常运作。回顾一下，谷仓由 $n$ 个房间组成，这些房间顺时针编号为 $1 \ldots n$，围绕谷仓的周边排列（$3 \leq n \leq 100$）。每个房间都有通往两个相邻房间的门，还有一扇门通向谷仓的外部。

Farmer John 希望最终有恰好 $r_i$ 头奶牛进入房间 $i$（$1 \leq r_i \leq 1,000,000$）。为了让奶牛有序地进入谷仓，他计划解锁 $k$ 扇外部门（$1 \leq k \leq 7$），只允许奶牛通过这些门进入。每头奶牛随后顺时针穿过房间，直到到达合适的目的地。Farmer John 希望解锁那些能让他的奶牛在进入谷仓后总共行走的距离最小的外部门（它们最初可以在 $k$ 扇解锁的门外任意排列；这不会计入总距离）。请确定如果他选择最佳的 $k$ 扇门解锁，他的奶牛需要行走的最小总距离。

### 输入格式

输入的第一行包含 $n$ 和 $k$。接下来的 $n$ 行每行包含 $r_1 \ldots r_n$。

### 输出格式

请输出奶牛需要行走的最小距离。

### 说明/提示

Farmer John 可以解锁门 2 和门 5。11 头奶牛从门 2 进入，总共行走 8 的距离到达房间 2、3 和 4。10 头奶牛从门 5 进入，总共行走 6 的距离到达房间 5、6 和 1。

```input1
6 2
2
5
4
2
6
2
```

```output1
14
```

## 提示
Farmer John can unlock doors 2 and 5.  11 cows enter at door 2 and walk a total distance of 8 to get to rooms 2, 3, and 4.  10 cows enter at door 5 and walk a total distance of 6 to get to rooms 5, 6 and 1.


