# AT_tkppc2016_c 有給休暇（Paid Vacation）

## 题目描述

Joisino 姐姐非常喜欢长假。

现在，已经知道了接下来的 $n$ 天是否是休息日。

Joisino 姐姐可以把最多 $k$ 个非休息日改为休息日。

Joisino 姐姐想知道可能的最长连续休息日的长度。

## 输入格式

第一行两个整数 $n,k$。

第二行 $n$ 个整数 $0$ 或 $1$，第 $i$ 个整数为 $1$ 表示第 $i$ 天是休息日，为 $0$ 表示第 $i$ 天是非休息日。

## 输出格式

输出最长连续休息日的长度。

## 输入输出样例 #1

### 输入 #1

```
6 2
1 0 1 0 0 1
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
10 1
1 1 0 0 1 1 1 0 1 1
```

### 输出 #2

```
6
```