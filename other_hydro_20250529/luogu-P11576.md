## 题目背景
本题译自 [Canadian Computing Competition](https://cemc.uwaterloo.ca/resources/past-contests?contest_category=29) [2020 Junior](https://cemc.uwaterloo.ca/sites/default/files/documents/2020/2020CCCJrProblemSet.html) T1 Dog Treats。

## 题目描述
小狗 Barley 喜欢零食。在一天结束时，他的心情取决于他在一天中收到的零食的大小与数量。

零食有三种大小：小、中、大。若这一天它获得小零食 $S$ 份，中零食 $M$ 份，大零食 $L$ 份，则他的快乐值可以用以下公式来衡量：

$1 \times S+2\times M + 3\times L$

如果 Barley 的快乐值大于等于 $10$，那么它是快乐的。否则，他会感到十分伤心。请判断 Barley 在一天结束时心情是快乐的还是伤心的。

## 输入格式
输入共 $3$ 行。

第一行一个整数 $S(0 \le S \le 10)$，表示小零食数量。

第二行一个整数 $M(0 \le M \le 10)$，表示中零食数量。

第三行一个整数 $L(0 \le L \le 10)$，表示大零食数量。

## 输出格式
一行一个字符串，若 Barley 的心情是快乐，则输出 `happy`，否则输出 `sad`。

```input1
3
1
0
```

```output1
sad
```

```input2
3
2
1
```

```output2
happy
```

## 提示
**本题采用捆绑测试**。

#### 【样例解释】
对于第一组样例，易得快乐值为 $1 \times 3+2\times 1 + 3\times 0=5$，而 $5< 10$，则 Barley 是伤心的。

对于第二组样例，易得快乐值为 $1 \times 3+2\times 2 + 3\times 1=10$，而 $10 \geq 10$，则 Barley 是快乐的。

