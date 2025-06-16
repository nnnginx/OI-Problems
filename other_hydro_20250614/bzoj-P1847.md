## 题目描述

有一些表达式本质上是相同的，如 `a+(b-c)`，`(a+b)-c`。你的任务是统计出 $N$ 元的不同表达式有多少个。

为使问题简单些，只有 `+`、`-`、`*`、`/` 和括号是允许的。

## 输入格式

一个整数 $N$，意义如上描述。

## 输出格式

一个整数表示表达式个数。

因为答案可能很大，只需输出对 $1000000007$ 取模后的值。

```input1
1
2
3
4
0

```

```output1
1
6
68
1170
```

## 样例说明

二元的表达式：

```
a+b, a-b, b-a, a*b, a/b, b/a
```

三元的表达式：

```
a+b+c, a+b-c, a-b+c, a-b-c, b-a+c, b-a-c, c-a-b
a*b*c, a*b/c, a/b*c, a/b/c, b/a*c, b/a/c, c/a/b
a+b*c, b+a*c, c+a*b,
a+b/c, a+c/b, b+a/c, b+c/a, c+a/b, c+b/a,
a-b*c, b-a*c, c-a*b,
a-b/c, a-c/b, b-a/c, b-c/a, c-a/b, c-b/a,
b*c-a, a*c-b, a*b-c,
b/c-a, c/b-a, a/c-b, c/a-b, a/b-c, b/a-c,
a*(b+c), b*(a+c), c*(a+b),
a*(b-c), a*(c-b), b*(a-c), b*(c-a), c*(a-b), c*(b-a),
a/(b+c), b/(a+c), c/(a+b),
a/(b-c), a/(c-b), b/(a-c), b/(c-a), c/(a-b), c/(b-a),
(b+c)/a, (a+c)/b, (a+b)/c,
(b-c)/a, (c-b)/a, (a-c)/b, (c-a)/b, (a-b)/c, (b-a)/c
```

注意四元的表达式中 `(a-b)/(c-d)` 和 `(b-a)/(d-c)` 是相同的，而 `a/b-c/d` 和 `b/a-d/c` 是不同的。

## 数据规模与约定

$N\le 30$。

