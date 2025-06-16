## 题目描述

这是一道模板题。

对于两个非负整数 $x, y$ 我们定义其 Nim 积 $x\otimes y$：

$$
x \otimes y = \operatorname {mex} \{ (a\otimes b) \oplus (a\otimes y) \oplus (x\otimes b) \mid 0\le a < x \wedge 0\le b < y  \}
$$

其中 $\oplus$ 是异或运算，$\operatorname{mex}$ 是集合中不存在的最小非负整数。


## 输入格式

第一行输入四个整数 $T, \mathrm{SA}, \mathrm{SB}, \mathrm{SC}$。

为了测试效率，询问数量 $T$ 可能很大，使用如下代码生成询问的输入：

```cpp
unsigned int SA, SB, SC;
unsigned int rng() {
    SA ^= SA << 16;
    SA ^= SA >> 5;
    SA ^= SA << 1;
    unsigned int t = SA;
    SA = SB;
    SB = SC;
    SC ^= t ^ SA;
    return SC;
}
```

在接下来 $T$ 组询问中，设 $\mathrm{lastans}$ 最初为 $0$，则按顺序有

```cpp
unsigned int x = rng() + lastans;
unsigned int y = rng();
lastans = nim_mul(x, y);
```

如此进行 $T$ 次循环。

## 输出格式

输出一行一个整数，表示最后一组解的答案。

```input1
5 171380702 78283356 95463589
```

```output1
1145338263
```

## 数据范围与提示

生成的数据均在 $2^{32}$ 范围以内，故保证 $0\le x, y < 2^{32}$。

四组数据中的 $T$ 分别为 $10, 1000, 3\times 10^4, 3\times 10^7$。

