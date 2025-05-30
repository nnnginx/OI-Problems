## 题目描述
蜗牛爬井问题：一只蜗牛要爬上 $v$ 米高的树桩，它每天白天向上爬 $a$ 米，晚上向下掉 $b$ 米。几天之后它可以爬到树桩顶？

## 输入格式
一行三个整数 $a$、$b$、$v$，用空格隔开。

## 输出格式
一行一个整数，表示答案。

```input1
2 1 5
```

```output1
4
```

```input2
5 1 6
```

```output2
2
```

```input3
100 99 1000000000
```

```output3
999999901
```

## 提示
#### 数据规模与约定

对于 $100\%$ 的数据，保证 $1 \leq  b < a \leq v \leq 1 \times 10^9$。

#### 说明

- 本题满分 $30$ 分。
- 题目译自 [COCI2010-2011](https://hsin.hr/coci/archive/2010_2011/) [CONTEST #2](https://hsin.hr/coci/archive/2010_2011/contest2_tasks.pdf) PUŽ，译者 @[mnesia](https://www.luogu.com.cn/user/115711)。

#### 提示

请推导结果公式，单纯的模拟可能导致 `TLE`。

