## 题目描述

__int64 ago,there's a heaven cow called sjy...

A god bull named wzc fell in love with her...

As an OI & MOer,wzc gave sjy a quesiton...

给定一个整数 $ n $，求一个整数 $ m $，满足 $ m\leq n $，并且 $ \dfrac{m}{\varphi(m)} $ 的值最大。

注： $ \varphi(m) $ 代表 $ m $ 的欧拉函数，即不大于 $ m $ 且与 $ m $ 互质的数的个数。

## 输入格式

第一行是一个整数 $ T $，表示该测试点有 $ T $ 组数据。
接下来 $ T $ 行，每行一个整数 $ n $，意义如上所述。

## 输出格式

输出一共 $ T $ 行，每行一个整数 $ m $。

若对于某个 $ n $，有不止一个满足条件的 $ m $，则输出最小的 $ m $。

## 样例输入

```
1
10
```

## 样例输出

```
6
```

## 数据规模与约定

对于 $100\%$ 的数据，$ T\leq 100 $，$ n\leq 10^{25000} $。

## 题目来源

Poetize3

