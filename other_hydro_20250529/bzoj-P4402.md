

## 题目描述
Claris 想要铸一把剑，这把剑必须符合他的审美，具体来说，我们可以把这把剑的不同地方的宽度看成一个序列，这个序列要满足以下条件：

+ 每个元素都是正整数（你的宽度不可能是负数吧）
+ 每个元素不能超过 $M$，太宽了如果比 Claris 身高还高怎么办（你可以认为 Claris 的身高就是 $M$）
+ 相邻两个元素的差的绝对值必须是 $1$（如果是 $0$，则这个地方不是锯齿，杀伤力不够，如果太大，又太丑了）
+ 第一个元素的值必须是 $1$（剑尖必须是最窄的地方）
他想知道有多少把长度不超过 $N$（即宽度的序列长度不超过 $N$）的合法的本质不同的剑。

我们认为两把剑本质不同，当且仅当存在至少一个宽度，在两把剑的宽度序列里面出现次数不一样。

比如 $\{1,2,3\}$ 和 $\{1,3,2\}$ 是本质相同的，但是 $\{1,2,3\}$ 和 $\{1,2,1\}$ 则是本质不同的。
## 输入格式
输入两个整数 $N,M$。
## 输出格式
只有一个整数，表示答案对 $10^9+7$ 取模的结果

```input1
5 3
```

```output1
9
```

## 样例解释
所有本质不同的合法的剑有如下：

$\{1\}$

$\{1,2\}$

$\{1,2,3\}$

$\{1,2,1\}$

$\{1,2,3,2\}$

$\{1,2,1,2\}$

$\{1,2,3,2,3\}$

$\{1,2,3,2,1\}$

$\{1,2,1,2,1\}$
## 数据规模与约定
对于 $100\%$ 的数据，$N,M \le 2\times 10^6$。

## 题目来源
By lyzy
