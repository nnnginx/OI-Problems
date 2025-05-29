## Description

You are given a hint to guess a positive number $x$, an integer ranging from $1$ to $n$.  


## Input

The first line contains a number $n$, indicating the range of the number (from $1$ to $n$).  
The second line contains a Python expression that implies $x$.

## Output

One integer $x$ to get full points. To get a few points without guessing, give a `0` as the answer.

For each case, write your answer into a file `date#.usr`. Either submit them directly within the editor on page, or pack all answer files into a single zip and upload it.

```input1
10
abs(x - 7) == 4
```

```output1
3
```

## Limits And Hints

本题中给出的 Python 表达式与 C++ 语义相同。表达式中 `x` 是一个整型变量，当 `x` 为正确答案时，表达式求值为 `True`；否则为 `False`。保证答案惟一。

注：
* Python 中 `a ** b` 表示计算 $a^b$。
* `pi` 的值为 $3.141592653589793$；三角函数使用弧度制。
* 给出的表达式可以直接在 Python 中 `from math import *` 后求值。
* 本题的测试数据中，`in` 文件是输出 $0$ 可得的分数百分比；`out` 文件是正确日期。在上传提交答案类题目时，如果 Special Judge 不需要 `in`/`out` 文件，可在 `data.yml` 中对应省略 `inputFile`/`outputFile` 项。
* **不保证** 答案是一个公历日期。

