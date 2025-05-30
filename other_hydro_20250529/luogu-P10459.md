## 题目描述
After successive failures in the battles against the Union, the Empire retreated to its last stronghold. Depending on its powerful defense system, the Empire repelled the six waves of Union's attack. After several sleepless nights of thinking, Arthur, General of the Union, noticed that the only weakness of the defense system was its energy supply. The system was charged by $N$ nuclear power stations and breaking down any of them would disable the system.

The general soon started a raid to the stations by $N$ special agents who were paradroped into the stronghold. Unfortunately they failed to land at the expected positions due to the attack by the Empire Air Force. As an experienced general, Arthur soon realized that he needed to rearrange the plan. The first thing he wants to know now is that which agent is the nearest to any power station. Could you, the chief officer, help the general to calculate the minimum distance between an agent and a station?


## 输入格式
The first line is a integer T representing the number of test cases.

Each test case begins with an integer $N (1 \leq N \leq 100000)$.

The next $N$ lines describe the positions of the stations. Each line consists of two integers $X (0 \leq X \leq 10^9)$ and $Y (0 \leq Y \leq 10^9)$ indicating the positions of the station.

The next following N lines describe the positions of the agents. Each line consists of two integers $X (0 \leq X \leq 10^9)$ and $Y (0 \leq Y \leq 10^9)$ indicating the positions of the agent.

## 输出格式
For each test case output the minimum distance with precision of three decimal placed in a separate line.

## 题目大意
**【题目描述】**

在连续的对抗联盟失败后，帝国撤退到了最后的要塞。依靠其强大的防御系统，帝国击退了联盟的六波攻击。经过几个不眠之夜的思考，联盟将军亚瑟注意到防御系统唯一的弱点是其能源供应。该系统由 $N$ 个核电站供电，破坏其中任何一个都会使系统失效。

将军很快派出了 $N$ 名特工突袭这些电站，他们被空投到了要塞内。不幸的是，由于帝国空军的袭击，他们未能着陆到预期的位置。作为一名经验丰富的将军，亚瑟很快意识到他需要重新安排计划。他现在想知道的第一件事是，哪个特工距离任何一个电站最近。作为首席官员，你能帮助将军计算特工与电站之间的最小距离吗？

**【输入格式】**

第一行是一个整数 $T$，表示测试用例的数量。

每个测试用例以一个整数 $N (1 \leq N \leq 100000)$ 开始。

接下来的 $N$ 行描述了电站的位置。每行包含两个整数 $X (0 \leq X \leq 10^9)$ 和 $Y (0 \leq Y \leq 10^9)$，表示电站的位置。

接下来的 $N$ 行描述了特工的位置。每行包含两个整数 $X (0 \leq X \leq 10^9)$ 和 $Y (0 \leq Y \leq 10^9)$，表示特工的位置。

**【输出格式】**

对于每个测试用例，输出距离最小值，保留三位小数，单独占一行。

翻译来自于：ChatGPT。

```input1
2
4 
0 0 
0 1 
1 0 
1 1 
2 2 
2 3 
3 2 
3 3 
4 
0 0 
0 0 
0 0 
0 0 
0 0 
0 0 
0 0 
0 0
```

```output1
1.414
0.000
```

