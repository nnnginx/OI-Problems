## 题目背景
JerryC最近迷上了狂野飙车！！！

## 题目描述
众所周知，JerryC是一位疯狂的Female。他最近买了一台跑车~~(但是却没有驾驶证)~~，所以他就只能到一个偏僻的地方练习开车。

当然，JerryC是不可能正常开车的。她首先决定要开$(B-A+1)$段路程的车，第$i$段路程的速度都是从$1$开始加速的。每一秒会加上$1$的单位速度。当速度加到$(i+A-1)$的时候，JerryC就会把速度降为$1$，然后开始下一段路程。

对于第$i$段路程的第$j$秒，JerryC获得的愉悦值为$\lfloor \frac{i+A-1}{j} \rfloor * (-1)^j$。(反正JerryC就是不喜欢奇数。)

现在请你求出JerryC最后的总愉悦值。

P.s. ：

如果上面的东西没有看懂，那么简单版就是这个意思：

给出A，B，求出下面式子的值。

$$\sum_{i=A}^B \sum_{j=1}^{i}\lfloor \frac{i}{j} \rfloor * (-1)^j$$

## 输入格式
一行，两个正整数A，B

## 输出格式
一行，一个整数表示最终的愉悦值。

```input1
1 1
```

```output1
-1
```

```input2
2 2
```

```output2
-1
```

```input3
3 3
```

```output3
-3
```

## 提示
对于50%的数据：$1 \leqslant A \leqslant B \leqslant 5*10^3$

对于70%的数据：$1 \leqslant A \leqslant B \leqslant 5*10^4$

对于100%的数据：$1 \leqslant A \leqslant B \leqslant 2*10^7$

