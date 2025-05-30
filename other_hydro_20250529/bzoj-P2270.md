## 题目描述

You are a hunter chasing a monkey in the forest，trying to shoot it down with your all-powerful automatic machine gun．The monkey is hiding somewhere behind the branches of one of the trees，out of your sight．You can aim at one of the trees and shoot；your bullets are capable of going through the branches and killing the monkey instantly if it happens to be in that tree．If it isn't，the monkey takes advantage of the time it takes you to reload and takes a leap into a neighbouring tree without you noticing．It never stays in the same place after a shot．You would like to find out whether there is an strategy that allows you to capture the monkey for sure，irrespective of its initial location and subsequent jumps．If so，you need to determine the shortest sequence of shots guaranteeing this．

As an example，consider the situation in which there are only two neighboring trees in the forest（left hand side of Figure 2）．It is then possible to make sure you capture the monkey by shooting twice at the same tree．Your first shot succeeds if the monkey happened to be there in the first place．Otherwise，the monkey was behind the other tree and it will necessarily have moved when you shoot for the second time．

However，depending on the shape of the forest it may not be possible for you to ensure victory．One example of this is if there are three trees，all connected to one another（right hand side of Figure 2）．No matter where you aim at，there are always two possible locations for the monkey at any given moment．（Note that here we are concerned with the worst-case scenario where the monkey may consistently guess your next target tree）．

你是一个在丛林中追逐猴子的猎人，你想用枪把猴子射下来。猴子藏在某棵树上，你是看不到它的。你可以向某棵树射击，若猴子在这棵树上它就完蛋了。若猴子不在，它就可以趁你装弹药的时候移动到某棵相邻的树上，而你无法发现它已转移。它一定不会在你射击之后停留在树上不动。你想要找到一种不管猴子的起始位置和跳法如何都一定可以杀死猴子的策略。请找出射击次数最少的方法。

举个例子，如果只有两棵相邻的树。你对着同一棵树射击两次就一定可以杀死猴子。如果人品好，第一次就可以杀死猴子。否则，第一次射击之后，猴子就一定会跳到第一次被射击的树上。第二次对着那棵树射击就可以杀死猴子了。

然而，丛林的复杂让你不一定可以获得胜利。一个例子就是有三棵树，互相连接。不管你打那一棵树，猴子总有两个地方可以跳（最坏情况是猴子可以预知你的下一个目标）。

## 输入格式

**本题有多组数据**

The input consists of several test cases，separated by single blank lines．Each test case begins with a line containing two integers $n$ and $m$；$n$ is the number of trees in the forest，and $m$ is the number of adjacency relations between trees．

Each of the following $m$ lines contains two distinct integers between 0 and $n-1$（inclusive），the identifiers of the trees in an adjacent pair．The order of both trees within a pair carries no meaning，and no pair appears more than once．You may further assume that no tree is adjacent to itself，and there is always a path between any two trees in the forest．

The test cases will finish with a line containing only two zeros （also preceded with a blank line）．

输入文件包含多组测试数据。每两组测试数据用空行隔开。

每个数据的第一行包含两个整数 $n$ 和 $m$。$n$ 表示树的棵数，$m$ 代表树之间的关系数。

接下来 $m$ 行，每行包含两个 $0$ 到 $n-1$ 之间的整数表示这两棵树是相邻的。每一对关系不会出现两次，没有树和自己连通，整个树林是连通的。
最后一行用两个零结束。

## 输出格式

Print a line for each test case．The line should contain the single word `Impossible` if the task is impossible．Otherwise，it must contain the shortest sequence of shots with the required property，in the format $L：V_1,V_2 \dots V_L$，where $L$ is the length of the sequence，and $V_1,V_2, \dots ,V_L$ are space-separated integers containing the identifiers of the trees to shoot at in the right order．If several shortest sequences exist，print the lexicographically smallest one（A sequence is smaller than another in lexicographic order if the first element on which they differ is smaller in the first one）．

每个测试数据输出一行。

如果打不死猴子输出 `Impossible`。否则，请输出射击次数最少的方案。格式为 $L：V_1,V_2 \dots V_L$。$L$ 代表射击次数，$V_1,V_2 \dots V_L$ 是每次射击的位置，用空格隔开。
如果有多组最优解，请输出字典序最小的。

```input1
2 1
0 1
3 3
0 1
1 2
2 0
4 3
0 1
2 3
1 3
```

```output1
2: 0 0
Impossible
4: 1 3 3 1
0 0
```

## 题目来源

鸣谢李青林

## 数据规模与约定

$100\%$ 的数据满足：$1 \le n \le 21$。