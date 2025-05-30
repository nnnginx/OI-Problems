## 题目描述
本题中，我们考察的是一类特殊的序列，这类序列只有 `+`，`-`（正号，负号）两种符号构成，比如：`-+++---++`。

我们将其中连续的 `+` 的长度按从左到右的顺序写出，即其派生序列，如 `-+++---++` 的派生序列为 $(3,2)$。

现在的问题是，我们已知一个序列 $A$ 的派生序列 $B$，但是 $A$ 的部分符号已经模糊到不能辨认的地步了。我们需要确定尽量多的符号。
## 输入格式
输入文件有两行。
第一行一个由 `+`，`-`，`?` 构成的序列，描述 $A$，其中 `?` 表示已经无法辨认的符号。
第二行有若干整数描述 $A$ 的生成序列 $B$。
## 输出格式
输出一行，一个序列描述你恢复后的序列 $A$（不能多余的空格），如果无解则输出一行 `No Solution`。
## 样例输入
```plain
+????-+??+
2 1 4
```
## 样例输出
```plain
++-??-++++
```
## 数据规模与约定
对于 $100\%$ 的数据，$|A| < 20001$，$B$ 的元素属于 $[1 \cdots |A|]$。
## 题目来源
第一届「NOIer」全国竞赛