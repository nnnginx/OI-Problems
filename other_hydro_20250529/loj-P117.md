## 题目描述

$ n $ 个点，$ m $ 条边，每条边 $ e $ 有一个流量下界 $ \text{lower}(e) $ 和流量上界 $ \text{upper}(e) $，给定源点 $ s $ 与汇点 $ t $，求源点到汇点的最小流。

## 输入格式

第一行两个正整数 $ n $、$ m $、$ s $、$ t $。

之后的 $ m $ 行，每行四个整数 $ s $、$ t $、$ \text{lower} $、$ \text{upper} $。

## 输出格式

如果无解，输出一行 `please go home to sleep`。

否则输出最小流。

```input1
7 12 6 7
6 1 0 2147483647
1 7 0 2147483647
6 2 0 2147483647
2 7 0 2147483647
6 3 0 2147483647
3 7 0 2147483647
6 4 0 2147483647
4 7 0 2147483647
6 5 0 2147483647
5 7 0 2147483647
5 1 1 2147483647
3 4 1 2147483647
```

```output1
2
```

## 数据范围与提示

$ 1 \leq n \leq 50003 , 1\leq m \leq 125003 $

