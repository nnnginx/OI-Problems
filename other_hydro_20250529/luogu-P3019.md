## 题目描述
Bessie and Jonell are great friends. Since Farmer John scrambles where the cows graze every day, they are sometimes quite far from each other and can't talk.

The pastures and paths on FJ's farm form a 'tree' structure.  Each pasture has exactly one distinct path to any other pasture, and each pasture (except pasture #1, the 'root') also has a single parent node.

Bessie and Jonell have decided that they will always meet at the closest pasture that that is both an ancestor of Jonell's pasture and of Bessie's pasture.

FJ created a map of his N (1 <= N <= 1,000) pastures (conveniently numbered 1..N) that tells the parent P\_i (1 <= P\_i <= N) of each pasture except pasture 1, which has no parent.

FJ has released his daily grazing schedule for the next M (1 <= M <= 1,000) days, so Bessie and Jonell are deciding where they should meet each day for gossip. On day k, Bessie is in pasture B\_k (1 <= B\_k <= N) and Jonell is in pasture J\_k (1 <= J\_k <= N).

Given a map and schedule, help Bessie and Jonell find their meeting places.

```cpp
Consider, for example, the following farm layout:

                            Pasture      Parent Pasture
             [1]           ---------    ----------------
            / | \              1              ---
           /  |  \             2               1 
         [2] [3] [6]           3               1
         /        | \          4               2
        /         |  \         5               8
      [4]        [8]  [9]      6               1
                /   \          7               8
               /     \         8               6
             [5]     [7]       9               6

Here are the meeting places that Bessie and Jonell would choose
given a six day schedule of their initial grazing locations:

              Bessie      Jonell       Meeting Place
             --------    --------     ---------------
                 2           7               1
                 4           2               2
                 1           1               1
                 4           1               1
                 7           5               8
                 9           5               6
```




## 输入格式
\* Line 1: Two space-separated integers: N and M

\* Lines 2..N: Line i contains a single integer that describes the parent of pasture i:  P\_i

\* Lines N+1..N+M: Line k+N describes Bessie and Jonell's respective pastures with two space-separated integers: B\_k and J\_k




## 输出格式
\* Lines 1..M: Line j contains the meeting place Bessie and Jonell would use for line j+N of the input


## 题目大意
农场是由N（1≤N≤1000）个节点组成的一棵树，1是树的根。有两头奶牛分别在两个节点，他们有M（1≤M≤1000）天要见面，见面地点在她们所在两个节点的路径上离根节点最近的节点。求出每天她们见面的节点编号。
输入：第一行两个整数N, M，接下来N-1行（这里的 i 是从 2 ~ n），第i行表示第i个节点的父亲编号，接下来M行每行两个整数表示当天两头奶牛所在的节点编号。
输出：输出M行，回答每个询问。

感谢@x咫尺天涯x 提供的翻译和ROY1994 提供的建议

```input1
9 6 
1 
1 
2 
8 
1 
8 
6 
6 
2 7 
4 2 
3 3 
4 1 
7 5 
9 5 

```

```output1
1 
2 
3 
1 
8 
6 

```

