## 题目描述
In the game, Deliv-e-droid, a robot droid has to deliver packages while avoiding obstacles.

At the end of the game, the final score is calculated based on the following point system:
- Gain $50$ points for every package delivered.
- Lose $10$ points for every collision with an obstacle.
- Earn a bonus $500$ points if the number of packages delivered is greater than the number of collisions with obstacles.

Your job is to determine the final score at the end of a game.


## 输入格式
The input will consist of two lines. The first line will contain a non-negative integer $P$,representing the number of packages delivered. The second line will contain a non-negative integer $C$,representing the number of collisions with obstacles.

## 输出格式
The output will consist of a single integer $F$,representing the final score.

## 题目大意
机器人 Deliv-e-droid 在送快递，如果它成功地将一个快递送达，则它获得 $50$ 元钱，如果未能成功送达，它被扣除 $10$ 元钱。特别地，如果它送达的快递的数量大于未送达的，它会得到 $500$ 元钱的奖励。

现在已知 Deliv-e-droid 送达了 $P$ 个快递，未送达 $C$ 个（$0 \leq P,C \leq 100$），请实现一个程序，求出 Deliv-e-droid 所获得的钱（如果是倒扣的话用负数表示）。

```input1
5
2
```

```output1
730
```

```input2
0
10
```

```output2
-100
```

