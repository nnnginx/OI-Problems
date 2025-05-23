# 题目背景

云斗纪 312 年，A、B  两个帝国开展了对两国领土过渡地带——卡纳卡地区的争夺战。当然，由于卡纳卡地区由许多摇摆不定的附属公国组成，所以这种争夺战必然是暗地里悄悄进行的。

A 帝国希望推动的战略是“王座下的背叛纲领”。你现在是 A 帝国国师的徒弟，A 帝国的国王便希望你来推动这个政策的运行。

# 题目描述

具体而言，卡纳卡地区可被视作一个长为 $w$ 、宽为 $h$ 的矩形。矩形中的 $w\times h$ 个元素代表卡纳卡地区的全部附属公国。

**一个公国要么服从 A 帝国，要么服从 B 帝国。** 当一个公国服从 A 帝国时，便会亮出 A 帝国的旗帜；反之，若服从 B 帝国，则亮出 B 帝国的旗帜。我们称这种亮出旗帜后的地图为**旗帜格局**。比如，一个也许会出现的旗帜格局如下：

```
A B A
B B B
```

这个旗帜格局会为你提供以下信息：

1. 卡纳卡地区的尺寸为 $2\times 3$，$w=2,h=3$，因此可被绘制为 $2$ 行 $3$ 列的矩阵。
2. 其中位于 $(1,1)$ 和 $(1,3)$ 的公国服从 A 帝国，位于 $(1,2),(2,1),(2,2),(2,3)$ 的公国服从 B 帝国。

而 A 国所谓的“王座下的背叛纲领”计划，便是暗地里派遣 A 帝国使者去某些公国进行游说。当 A 帝国使者游说到某个公国时，该公国四连通(即上、下、左、右连通)的其他公国会得知此事。由于公国在帝国面前的力量实在是太渺小，这些公国都会因为压力过大而直接**倒戈**。也就是说，**当 A 帝国使者游说到某个公国时，该公国及其四连通(即上、下、左、右连通)的相邻公国会立即调换阵营**。

例如，在以下旗帜格局里，某次 A 帝国大使游说到了公国 $(1,2)$：

```
A B A
B B B
```

那么根据以上信息，公国 $(1,2)$ 和他的四连通邻国 $(1,1),(1,3),(2,2)$ 都会倒戈。因此卡纳卡地区的旗帜格局会变为

```
B A B
B A B
```

兵贵神速，但 A 帝国大使的游说显然需要时间。因此，A 帝国的国王希望你能够设计一个策略，用**最少的游说次数**让全部公国**都服从于 A 帝国**，也即让全部公国都亮出 A 帝国的旗帜。

现在你需要回答，在你的最优设计下，A 帝国大使至少需要几次游说才能完成任务。

注意，B 国是**不会**来捣乱的哦~

# 输入格式

第一行为一个整数 $T$ 表示数据组数。

接下来每组数据：

第 $1$ 行共两个整数 $w,h$，分别表示卡纳卡地区的长度与宽度。

第 $2$ 至 $w + 1$ 行，每行 $h$ 个大写字母 $A$ 或 $B$，用于描述当前卡纳卡地区的旗帜格局。

# 输出格式

共 $T$ 行，每行为一个整数，表示相应数据的最佳答案，保证有解。

# 样例

### 样例输入 #1

```
2
1 10
B B B B B B B B B B
3 5
B B A A B
A A B A B
A A B A B
```

### 样例输出 #1

```
4
3
```

### 样例输入 #2

```
3
3 3
A B B
A A B
B B A
4 6
B A A A B A
A A B A A A
B A A A A B
B B B B B B
10 2
B B
A A
B A
B A
B A
A A
A B
A A
A B
A B

```

### 样例输出 #2

```
4
12
11
```

# 提示

## 样例说明

第一组数据，可以选择游说 $(1,1),(1,4),(1,7),(1,10)$，得到最小游说次数 $4$ 。

第二组数据，可以选择游说$(1,2),(2,3),(2,5)$，得到最小游说次数 $3$ 。

## 数据规模与约定

对于 $20\%$ 的测试点，保证 $1 ≤ w × h ≤ 25$。

另有 $30\%$ 的测试点，保证 $1\leq w \leq  2$。

对于 $100\%$的测试点，保证 $1 ≤ T ≤ 8，1 ≤ w ≤ 10，1 ≤ h ≤ 1200$。

