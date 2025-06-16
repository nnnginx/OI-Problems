## 题目描述
Bessie and Elsie have each baked $N$ pies ($1 \leq N \leq 10^5$). Each of the $2N$ pies has a tastiness value according to Bessie and a (possibly different) tastiness value according to Elsie.

Bessie is thinking about giving one of her pies to Elsie. If Elsie receives a pie from Bessie, she will feel obligated to give one of her pies to Bessie. So as to not appear stingy nor flamboyant, Elsie will try to pick a pie that is at least as tasty (in Elsie's eyes) as the pie she received, but no more than $D$ units tastier ($0 \leq D \leq 10^9$). Such a pie may not exist, in which case Elsie will adopt a pseudonym and exile herself to Japan.


But if Elsie does give Bessie a pie in return, Bessie will similarly try to give Elsie a pie which is at least as tasty but no more than $D$ units tastier (in Bessie's eyes) as the pie Elsie just gave her. Should this be impossible, Bessie too will exile herself. Otherwise she will give her chosen pie to Elsie. This cycle will continue until one of the cows is exiled, an unhappy outcome, or one of the cows receives a pie which she accords a tastiness value of $0$, in which case the gift exchange will end and both cows will be happy.


Note that a pie may not be gifted twice, nor can either cow return a pie gifted to her.


For each of the $N$ pies Bessie could select as her initial gift to Elsie, determine the minimum number of pies that could possibly be gifted in the resulting exchange before the cows are happy.


## 输入格式
The first line contains the two integers $N$ and $D$.

The next $2N$ lines contain two space-separated integers each, respectively denoting the value of a particular pie according to Bessie, and the value of that pie according to Elsie.


The first $N$ lines refer to Bessie's pies, and the remaining $N$ lines refer to Elsie's pies.


It is guaranteed that all tastiness values are in the range $[0,10^9]$.


## 输出格式
There should be $N$ lines in the output. Line $i$ should contain a single integer: the minimum number of pies that could be gifted in a happy gift exchange started with Bessie's pie $i$. If no gift exchange starting with pie $i$ is happy, then line $i$ should contain the single integer $-1$ instead.


## 题目大意
### 题目描述

Bessie 和 Elsie 各自烤了 $N$ 个派（$1 \leq N \leq 10^5$）。这 $2N$ 个派中的每一个都有一个由 Bessie 评定的美味值和一个（可能不同的）由 Elsie 评定的美味值。

Bessie 正在考虑将她的一只派送给 Elsie。如果 Elsie 收到了 Bessie 的派，她会觉得有义务回赠 Bessie 一只派。为了既不显得吝啬也不显得炫耀，Elsie 会尝试选择一只在她看来至少与收到的派一样美味，但不超过 $D$ 单位更美味的派（$0 \leq D \leq 10^9$）。如果这样的派不存在，Elsie 将采用一个化名并自我流放到日本。

但如果 Elsie 确实回赠了 Bessie 一只派，Bessie 也会类似地尝试送给 Elsie 一只在她看来至少与 Elsie 刚送给她的派一样美味，但不超过 $D$ 单位更美味的派。如果这不可能，Bessie 也会自我流放。否则，她会将她选择的派送给 Elsie。这个循环将继续，直到其中一头奶牛被流放（一个不愉快的结果），或者其中一头奶牛收到一只她评定美味值为 $0$ 的派，在这种情况下，礼物交换将结束，两头奶牛都会感到高兴。

请注意，一只派不能被赠送两次，任何一头奶牛也不能回赠她收到的派。

对于 Bessie 可以选择作为初始礼物送给 Elsie 的每一只派，确定在奶牛们感到高兴之前，可能被赠送的派的最小数量。

### 输入格式

第一行包含两个整数 $N$ 和 $D$。

接下来的 $2N$ 行每行包含两个用空格分隔的整数，分别表示某只派由 Bessie 评定的美味值和由 Elsie 评定的美味值。

前 $N$ 行描述 Bessie 的派，剩下的 $N$ 行描述 Elsie 的派。

保证所有美味值都在 $[0,10^9]$ 范围内。

### 输出格式

输出应包含 $N$ 行。第 $i$ 行应包含一个整数：如果以 Bessie 的第 $i$ 只派开始的礼物交换是高兴的，则输出可能被赠送的派的最小数量；否则输出 $-1$。

```input1
2 1
1 1
5 0
4 2
1 4
```

```output1
3
1

```

