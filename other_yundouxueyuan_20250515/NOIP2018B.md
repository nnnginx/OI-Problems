# Description

轩轩和凯凯正在玩一款叫《龙虎斗》的游戏，游戏的棋盘是一条线段，线段上有 𝑛
个兵营（自左至右编号 1 ~ 𝑛），相邻编号的兵营之间相隔 1 厘米，即棋盘为长度为
𝑛 − 1 厘米的线段。𝑖 号兵营里有 c𝑖 位工兵。
下面图 1 为 𝑛 = 6 的示例：
![image](./4182/file/dxbBrcCXKZwoTc00oKvMV.png) 图 1. 𝑛 = 6的示例
轩轩在左侧，代表“龙”；凯凯在右侧，代表“虎”。 他们以 m 号兵营作为分界，
靠左的工兵属于龙势力，靠右的工兵属于虎势力，而第 𝐦 号兵营中的工兵很纠结，他
们不属于任何一方。
一个兵营的气势为：该兵营中的工兵数 × 该兵营到 m 号兵营的距离；参与游戏
一方的势力定义为：属于这一方所有兵营的气势之和。
下面图 2 为 n = 6, 𝑚 = 4 的示例，其中红色为龙方，黄色为虎方：
![image](./4182/file/YBKs3NXWwyC1_JPd9sZsB.png) 图 2. n = 6, 𝑚 = 4的示例
游戏过程中，某一刻天降神兵，共有 𝑠1 位工兵突然出现在了 𝑝1 号兵营。作为轩
轩和凯凯的朋友，你知道如果龙虎双方气势差距太悬殊，轩轩和凯凯就不愿意继续玩下
去了。为了让游戏继续，你需要选择一个兵营 𝑝2，并将你手里的 𝑠2 位工兵全部派往
兵营 𝑝2，使得双方气势差距尽可能小。
注意：你手中的工兵落在哪个兵营，就和该兵营中其他工兵有相同的势力归属（如
果落在 m 号兵营，则不属于任何势力）

# Format

## Input

输入文件名为 fight.in。
输入文件的第一行包含一个正整数 𝑛，代表兵营的数量。
接下来的一行包含 𝑛 个正整数，相邻两数之间以一个空格分隔，第 𝑖 个正整数代
表编号为 𝑖 的兵营中起始时的工兵数量 𝑐𝑖。
接下来的一行包含四个正整数，相邻两数间以一个空格分隔，分别代表 𝑚, 𝑝1, 𝑠1, 𝑠2。

## Output

输出文件名为 fight.out。
输出文件有一行，包含一个正整数，即 𝑝2，表示你选择的兵营编号。如果存在多
个编号同时满足最优，取最小的编号。

# Samples

```input1
6
2 3 2 3 2 3
4 6 5 2
```

```output1
2
```

```input2
6
1 1 1 1 1 16 
5 4 1 1
```

```output2
1
```

# Limitation

【输入输出样例 1 说明】
见问题描述中的图 2。
双方以 𝑚 = 4 号兵营分界，有 𝑠1 = 5 位工兵突然出现在 𝑝1 = 6 号兵营。
龙方的气势为：
2 × (4 − 1) + 3 × (4 − 2) + 2 × (4 − 3) = 14
虎方的气势为：
2 × (5 − 4) + (3 + 5) × (6 − 4) = 18
当你将手中的 𝑠2 = 2 位工兵派往 𝑝2 = 2 号兵营时，龙方的气势变为：
14 + 2 × (4 − 2) = 18
此时双方气势相等
【输入输出样例 2 说明】
双方以 𝑚 = 5 号兵营分界，有 𝑠1 = 1 位工兵突然出现在 𝑝1 = 4 号兵营。
龙方的气势为：
1 × (5 − 1) + 1 × (5 − 2) + 1 × (5 − 3) + (1 + 1) × (5 − 4) = 11
虎方的气势为：
16 × (6 − 5) = 16
当你将手中的 𝑠2 = 1 位工兵派往 𝑝2 = 1 号兵营时，龙方的气势变为：
11 + 1 × (5 − 1) = 15
此时可以使双方气势的差距最小。
【输入输出样例 3】
见选手目录下的 fight/fight3.in 和 fight/fight3.ans。
【数据规模与约定】
1 < 𝑚 < 𝑛, 1 ≤ 𝑝1 ≤ 𝑛。
对于 20% 的数据，𝑛 = 3, 𝑚 = 2, 𝑐𝑖 = 1, 𝑠1, 𝑠2 ≤ 100。
另有 20% 的数据，𝑛 ≤ 10, 𝑝1 = 𝑚, 𝑐𝑖 = 1, 𝑠1, 𝑠2 ≤ 100。
对于 60% 的数据，𝑛 ≤ 100, 𝑐𝑖 = 1, 𝑠1, 𝑠2 ≤ 100。
对于 80% 的数据，𝑛 ≤ 100, 𝑐𝑖, 𝑠1, 𝑠2 ≤ 100。
对于 100% 的数据，𝑛 ≤ 105, 𝑐𝑖, 𝑠1, 𝑠2 ≤ 109。

