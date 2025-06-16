# AT_rcl_contest_2021_b マッサージチェア2021

## 题目描述

在 X 先生工作的办公室闲置区，排列着一个 $N \times N$ 的按摩椅矩阵。每个按摩椅的位置用 $(i, j)$ 表示，其中 $i$ 是行号，$j$ 是列号。

这些按摩椅具有不同的**性能**。位于 $(i, j)$ 处的按摩椅的**性能**用 $1$ 到 $30$ 之间的整数 $E_{i, j}$ 表示，数值越大表示性能越好。此外，按摩椅的**功率**可以自由设置为 $0$ 到 $N$ 之间的整数，记为 $P_{i, j}$。

- 将**功率**设置为 $0$ 的按摩椅不会被使用，没人会坐。
- 将**功率**设置为非零值的按摩椅必须有人坐。
- 若按摩椅的**功率**设为 $P_{i, j}$（非零），则位于该按摩椅曼哈顿距离不超过 $P_{i, j}$ 距离内的其他按摩椅不得有人坐，因为会受到**噪音**影响。

下图示例展示了对部分按摩椅设置非零**功率**的情况。方格内的数字表示该位置按摩椅的**功率**，粉色方格中的按摩椅需保持无人使用。

![](data:image/png;base64,%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.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ägTMN5SqrIxVd5HcmHd5/V9W2uNBA4dPzZeryc3/HRPbR7jIhxzIhxzIhxzIhxzIhxzIhxzIhxzIhxzIhxzIhxzIhxzIhxzIhxzIhxzIhxzIixzam4iKQGiFGi487L7goMSyEUgoRQgoTVZhrn0/ibuSzuepXJ71k6As3SVTDdtKE7QSuYmlkNIJ8W7eF7nvFVw3nX3PayijdYaArbA1xxekk5Xb8tYr+Y6mV8dJ/U9YiPF56Dv2uA8Avj9V6DgayHgBof4+7Q9TiOIo7y6A+fWYAmrufXSvoS+k1+Gaeva6SEFATAzEAQgAoARCACgIBEIAKAEQgAoARCACgBEAtw7o/yy+Bi/pHroit09PuFJPKfHn+dHvrMxawF5ZIEQEAOgnwPQI8D4f+XkuJHZWR0AAAAASUVORK5CYII=)

在 X 先生为每个按摩椅设置**功率**后，所有**功率**不为 $0$ 的按摩椅将会有人坐在上面。坐在位于 $(i, j)$ 处按摩椅上的人将会获得的满意度为 $E_{i, j} \times P_{i, j}$。请尽可能地使所有坐在按摩椅上的人满意度之和达到最大。

各测试用例得分以及这一题的总得分计算方式如下：

- 对于每个测试用例，所有坐在按摩椅上的人的满意度总和即为得分。
- 总共有 $50$ 个测试用例，每个测试用例得分的总和即为问题的总得分。

## 输入格式

输入通过标准输入给出，格式如下：

```
\(\begin{array}{lll}
    N & & \\
    E_{ 0,0 } & \ldots & E_{ 0,N-1 } \\
    \vdots & \ddots & \vdots \\
    E_{ N-1,0 } & \ldots & E_{ N-1,N-1 }
  \end{array}\)
```

- $N$ 表示按摩椅的行数和列数，总数为 $N = 40$。
- $E_{i, j}$ 表示第 $(i, j)$ 个按摩椅的**性能**，满足 $1 \leq E_{i, j} \leq 30$。

## 输出格式

请输出 $N$ 行，每行含有 $N$ 个整数，作为标准输出：

```
\(\begin{array}{lll}
    P_{ 0,0 } & \ldots & P_{ 0,N-1 } \\
    \vdots & \ddots & \vdots \\
    P_{ N-1,0 } & \ldots & P_{ N-1,N-1 }
  \end{array}\)
```

- $P_{i, j}$ 代表第 $(i, j)$ 个按摩椅的**功率**，必须小于等于 $N$。
- 受到**噪音**影响的按摩椅的**功率**必须设置为 $0$。
- 如果输出结果不符合上述要求，将判定为 WA。

## 提示

### 测试用例生成说明

所有测试用例由一个测试用例生成器生成，可以通过链接获得。生成器按照以下方法生成用例，具体实现请查看代码：

- 使 $E_{i, j}$ 取值为 $x$ 的概率与 $1/x^2$ 成正比，因此 $E_{i, j}$ 的值越大，其出现频率越低。

### 提供的文件

提供了测试用例生成器、测试工具、样例数据和可视化工具：

[测试用例生成器、测试工具、样例输入数据和可视化工具 (zip)](https://img.atcoder.jp/rcl-contest-2021/005883cbd767ff24197df17a19959035.zip)

### 可视化工具说明

我们提供了一个工具可以可视化输入输出的数据和得分。

- 本工具在最新版本的桌面版 [Google Chrome](https://www.google.co.jp/chrome/) 和 [Mozilla Firefox](https://www.mozilla.org/firefox/new/) 上进行了测试，但不能保证在所有浏览器上兼容。
- 工具计算的得分并不代表比赛中的实际得分，解答需通过提交到 AtCoder 完成评分。此外，工具计算的得分并不保证与比赛最终得分一致。
- 因使用该工具造成的任何损失概不负责。

可视化工具和使用说明包含在提供的文件中，详情请查阅文件中的 README.html。

### 样例说明

- 样例 1 由于演示用，不符合输入约束（$N = 40$），得分计算为 $2 \times 1 + 5 \times 1 + 16 \times 4 = 71$。注意，**功率**不能大于 $N$。

- 样例 2 与测试工具中附带的 `input_0.txt` 相同，在这里省略输出示例。

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
4
1 2 3 4
5 6 7 8
9 10 11 12
13 14 15 16
```

### 输出 #1

```
0 1 0 0
1 0 0 0
0 0 0 0
0 0 0 4
```

## 输入输出样例 #2

### 输入 #2

```
40
4 2 1 1 1 1 3 1 1 1 6 1 1 2 1 1 6 17 3 5 1 2 5 2 1 1 1 1 6 12 1 4 1 3 1 1 2 1 3 2
1 1 4 1 1 4 1 1 1 12 3 1 1 1 1 7 1 1 2 1 3 1 11 1 1 1 1 1 1 1 1 1 1 2 1 1 2 4 6 3
5 6 1 1 2 1 3 4 5 1 9 1 1 2 26 6 3 1 1 1 2 4 1 2 1 1 3 1 3 1 1 2 1 1 6 1 2 1 2 1
1 1 1 16 1 1 10 1 1 1 3 7 1 1 1 1 1 2 1 1 1 1 1 19 1 1 2 3 6 1 2 12 1 2 4 1 1 1 1 1
1 1 1 1 1 1 3 1 1 1 2 1 1 1 1 9 1 1 1 8 2 2 2 1 1 2 1 1 1 1 2 1 4 1 1 1 2 1 2 1
1 1 1 1 1 1 2 5 1 1 1 3 4 3 1 30 2 1 2 19 1 2 1 1 2 1 3 1 1 1 2 4 1 15 1 4 1 1 1 1
3 4 1 1 2 1 4 1 1 1 2 1 8 8 6 1 2 2 2 2 5 2 1 1 1 1 1 1 1 3 2 1 2 1 1 16 1 1 1 1
1 1 1 1 1 1 1 1 1 1 6 1 3 14 1 1 2 1 1 2 5 6 2 1 14 2 1 1 2 1 1 1 1 1 1 1 2 1 1 19
1 3 1 1 1 4 2 5 1 2 1 1 1 1 9 1 1 1 1 1 1 20 17 1 1 2 4 1 6 1 1 1 2 1 1 1 1 11 5 3
1 1 1 3 3 1 2 3 1 1 4 1 1 1 1 3 1 1 1 2 12 1 5 1 1 2 3 2 21 2 5 1 1 1 3 1 3 1 1 4
3 2 1 1 1 1 1 4 8 1 1 3 1 2 1 1 3 1 1 1 1 4 2 2 1 18 1 1 1 1 1 1 1 1 2 1 1 1 1 3
1 4 1 1 2 1 1 2 2 3 1 6 3 6 4 2 3 1 3 1 3 1 2 1 3 1 1 7 1 5 8 2 1 1 1 3 5 3 2 1
1 1 1 1 6 7 1 1 2 2 1 1 2 1 6 11 2 1 1 1 1 1 1 13 3 1 5 1 1 2 8 1 1 1 1 1 4 1 1 1
10 1 12 1 1 1 7 10 2 1 23 1 1 1 5 8 3 1 1 2 1 1 1 1 1 1 1 1 1 2 1 1 2 1 1 1 9 1 1 1
2 1 1 1 1 9 3 1 1 2 3 1 1 2 1 1 1 7 1 1 2 1 1 1 2 1 1 1 2 2 1 1 2 1 2 2 1 2 1 17
1 5 1 1 1 1 1 1 1 1 2 6 1 1 3 1 1 1 1 6 1 1 1 1 1 2 1 1 2 1 3 3 1 1 2 1 2 1 1 1
2 1 1 1 1 2 1 2 1 1 2 1 2 1 1 5 1 1 1 4 2 2 2 1 1 2 30 4 2 2 1 2 1 1 1 1 1 1 5 1
1 2 1 1 6 1 3 1 3 1 1 1 8 1 1 1 1 1 1 1 2 1 1 1 2 1 1 4 1 1 2 1 10 9 7 7 1 1 2 1
1 1 1 1 2 1 3 2 12 1 6 1 1 1 4 3 1 1 1 1 1 1 1 1 1 1 2 2 1 4 1 1 2 1 7 1 1 2 1 3
15 1 1 1 1 2 1 6 1 1 1 2 3 1 1 1 1 4 7 1 1 1 1 1 1 1 1 1 1 1 1 1 3 1 2 1 1 2 2 2
1 4 1 2 1 2 1 2 2 2 1 3 1 1 2 1 2 1 1 3 1 1 1 1 1 1 14 1 1 2 3 2 1 2 1 2 3 2 1 1
2 5 1 3 1 1 1 1 1 2 2 1 9 1 1 4 1 1 2 3 3 1 1 1 2 11 1 1 2 2 1 2 1 1 1 2 1 1 2 1
1 1 2 1 1 13 1 5 1 1 1 1 1 18 2 1 1 1 1 2 2 1 1 6 1 1 1 1 4 1 2 1 1 3 3 1 1 3 1 3
2 1 1 7 1 2 1 1 1 1 3 2 1 7 1 1 1 1 1 1 2 1 1 1 1 1 5 1 14 2 1 1 2 1 2 1 1 1 2 1
2 1 3 1 2 1 1 1 15 13 1 1 1 12 6 1 2 2 1 6 5 1 2 1 3 1 9 1 2 1 3 1 19 1 1 1 1 7 9 1
8 3 3 2 1 1 1 9 1 1 2 1 1 1 3 1 2 1 1 1 21 2 8 1 1 21 1 3 3 4 2 1 2 6 1 1 9 1 1 1
3 1 1 1 8 2 2 2 1 2 1 5 1 8 7 1 1 2 1 1 3 2 10 1 6 7 2 8 1 4 2 1 1 1 1 1 2 1 3 2
1 4 1 1 3 1 2 1 1 1 1 1 1 1 1 1 1 1 1 7 4 8 1 5 17 2 1 2 1 1 1 1 1 1 1 2 2 1 3 1
1 2 2 9 1 1 1 1 3 1 1 2 1 1 7 28 1 5 1 1 1 2 1 2 3 1 2 1 1 1 1 1 2 1 1 1 3 1 3 1
1 1 1 3 1 19 4 1 1 1 2 1 5 1 1 1 1 1 1 2 2 1 3 1 1 1 5 2 2 1 3 1 1 3 1 1 1 1 1 1
1 2 1 1 1 4 1 1 1 4 3 4 1 2 1 3 1 10 1 1 6 2 1 1 1 1 1 1 1 6 2 1 4 2 8 1 5 2 1 1
1 1 1 1 4 1 4 1 1 1 7 1 1 3 30 1 3 1 1 3 1 1 3 2 1 1 1 6 1 1 1 1 1 1 1 2 11 1 1 1
1 1 2 1 1 3 28 5 1 1 1 1 1 1 1 3 11 1 4 1 2 1 1 4 1 6 2 1 1 1 1 1 26 1 1 7 1 2 2 2
2 1 10 1 1 1 2 1 1 2 1 2 1 1 1 1 1 1 1 2 2 3 1 1 1 1 1 1 3 1 4 2 2 1 1 11 4 1 4 5
1 1 1 2 6 17 2 1 4 22 1 9 1 11 25 3 2 1 1 1 2 7 1 2 2 1 2 16 1 2 1 1 3 1 5 3 1 1 1 1
1 1 3 6 1 3 1 4 6 1 3 4 4 1 1 1 2 1 1 1 1 5 1 6 7 1 1 1 1 1 1 1 3 1 2 1 1 1 1 4
3 1 1 1 1 9 1 1 1 1 1 3 1 4 3 1 1 1 4 1 2 1 2 7 1 4 1 1 1 1 3 1 1 1 8 1 1 1 1 1
1 1 2 1 7 2 1 4 1 1 1 3 1 1 1 2 1 6 1 1 1 2 23 4 1 1 1 1 1 1 10 1 1 1 1 1 15 14 1 1
2 1 1 1 2 1 1 5 1 12 17 1 1 1 1 1 1 3 1 1 1 1 1 1 1 7 1 2 1 1 5 4 1 1 1 7 1 3 1 1
2 1 1 1 2 3 2 2 1 1 8 2 1 2 2 2 1 1 2 1 1 1 1 6 1 5 1 1 1 1 1 1 1 3 1 1 1 7 1 2
```

### 输出 #2

```

```