## 题目描述

黑白棋游戏是这样玩的：首先 GEN 随机生成 $n$ 个 `01` 序列，`0` 表示白棋，`1` 表示黑棋。接着两个人轮流按如下规则取棋：首先选取一个非空的 `01` 序列，然后从该序列的左边开始连续取若干个棋子，这些被取的棋子中最多只能有 一个黑棋，且该黑棋必需恰好是连续取的最后一个棋子，比如当前的序列为 `001001`，则可以取走的棋子有三种情况，分别为：`0`，`00`，`001`。如果某人没有棋子可取了，则他负。

你通过特殊手段得到了 GEN 生成时每一行生成的白棋数目和黑棋数目，由于不知道它们的排列情况，你做不到必胜，你只想知道你先手获胜的概率有多大(假设你和你的对手都无限聪明)。

## 输入格式

第一行一个数 $n$。

第二行 $n$ 个数，第 $i$ 个数表示第 $i$ 个 `01` 序列中黑棋的个数。

第三行 $n$ 个数，第 $i$ 个数表示第 $i$ 个 `01` 序列中白棋的个数。

## 输出格式

仅一行，一个保留 $6$ 位小数的的实数表示先手获胜的概率。

```input1
1
1
1
```
```output1
0.500000
```
## 样例说明 1

若生成序列为 `01`，则先手必胜；若生成序列为 `10`，则后手必胜。

两种情况出现的概率均为 $0.5$，故先手获胜的概率为 $0.5$。

## 数据规模与约定

对于 $100\%$ 的数据，$0 \leq  $ 每行的黑棋个数 $ \leq 100$，$0 \leq  $ 每行的白棋个数 $ \leq 100$，$1 \leq n \leq 50$，数据保证每个序列至少有一个棋子。