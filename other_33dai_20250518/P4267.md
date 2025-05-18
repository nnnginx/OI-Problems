## 题目描述
Early in the morning, Farmer John woke up to the sound of splintering wood. It was the cows, and they were breaking out of the barn again!
Farmer John was sick and tired of the cows' morning breakouts, and he decided enough was enough: it was time to get tough. He nailed to the barn wall a counter tracking the number of days since the last breakout. So if a breakout occurred in the morning, the counter would be $0$ that day; if the most recent breakout was $3$ days ago, the counter would read $3$. Farmer John meticulously logged the counter every day.

The end of the year has come, and Farmer John is ready to do some accounting. The cows will pay, he says! But something about his log doesn't look quite right...

Farmer John wants to find out how many breakouts have occurred since he started his log. However, he suspects that the cows have tampered with his log, and all he knows for sure is that he started his log on the day of a breakout. Please help him determine, for each number of breakouts that might have occurred since he started the log, the minimum number of log entries that must have been tampered with.

## 输入格式
The first line contains a single integer $N$ ($1 \leq N \leq 100$), denoting the number of days since Farmer John started logging the cow breakout counter.
The second line contains $N$ space-separated integers. The $i$th integer is a non-negative integer $a_i$ (at most $100$), indicating that on day $i$ the counter was at $a_i$, unless the cows tampered with that day's log entry.

## 输出格式
The output should consist of $N$ integers, one per line. The $i$th integer should be the minimum over all possible breakout sequences with $i$ breakouts, of the number of log entries that are inconsistent with that sequence.

## 题目大意
### 题目描述

清晨，Farmer John 被木头碎裂的声音吵醒。原来是奶牛们又一次从谷仓里逃出来了！
Farmer John 对奶牛们的清晨逃跑行为感到厌烦，他决定受够了：是时候采取强硬措施了。他在谷仓的墙上钉了一个计数器，用于记录自上次逃跑以来的天数。因此，如果某天早上发生了逃跑，计数器当天会显示 $0$；如果最近一次逃跑发生在 $3$ 天前，计数器会显示 $3$。Farmer John 每天都会仔细记录计数器的值。

年末到了，Farmer John 准备进行一些统计。他说，奶牛们要为此付出代价！但他发现他的记录似乎有些不对劲……

Farmer John 想知道自从他开始记录以来发生了多少次逃跑。然而，他怀疑奶牛们篡改了他的记录，他唯一能确定的是他开始记录的那天发生了一次逃跑。请帮助他确定，对于可能发生的逃跑次数，记录中必须被篡改的最小条目数。

### 输入格式

第一行包含一个整数 $N$（$1 \leq N \leq 100$），表示 Farmer John 开始记录奶牛逃跑计数器以来的天数。
第二行包含 $N$ 个以空格分隔的整数。第 $i$ 个整数是一个非负整数 $a_i$（最多 $100$），表示第 $i$ 天计数器的值为 $a_i$，除非奶牛篡改了那天的记录。

### 输出格式

输出应包含 $N$ 个整数，每行一个。第 $i$ 个整数应表示在所有可能的逃跑序列中，发生 $i$ 次逃跑时，与序列不一致的记录条目的最小数量。

### 提示

如果只有 $1$ 次逃跑，那么正确的记录应该是 `0 1 2 3 4 5`，这与给定的记录有 $4$ 个条目不同。

如果有 $2$ 次逃跑，那么正确的记录可能是 `0 1 2 3 0 1`，这与给定的记录有 $2$ 个条目不同。在这种情况下，逃跑发生在第 $1$ 天和第 $5$ 天。

如果有 $3$ 次逃跑，那么正确的记录可能是 `0 1 2 0 0 1`，这与给定的记录只有 $1$ 个条目不同。在这种情况下，逃跑发生在第 $1$ 天、第 $4$ 天和第 $5$ 天。

以此类推。

题目来源：Brian Dean 和 Dhruv Rohatgi

```input1
6
1 1 2 0 0 1
```

```output1
4
2
1
2
3
4
```

## 提示
If there was only 1 breakout, then the correct log would look like 0 1 2 3 4 5, which is 4 entries different from the given log.

If there were 2 breakouts, then the correct log might look like 0 1 2 3 0 1, which is 2 entries different from the given log. In this case, the breakouts occurred on the first and fifth days.

If there were 3 breakouts, then the correct log might look like 0 1 2 0 0 1, which is just 1 entry different from the given log. In this case, the breakouts occurred on the first, fourth, and fifth days.

And so on.

Problem credits: Brian Dean and Dhruv Rohatgi

