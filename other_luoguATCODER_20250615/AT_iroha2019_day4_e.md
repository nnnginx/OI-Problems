# AT_iroha2019_day4_e 芽生え

## 题目描述

### 题目大意
有N张桌子，每张桌子上可以有若干个（$0 \le 数量 \le K$）苹果。

两个人轮流选一张桌子拿至少1个苹果，不能不拿，谁先拿完谁获胜。两人均采取最优策略。

请设置每张桌子的苹果数量，使先手必胜。输出总方案数量。

## 输入格式

只有一行，包含两个整数N（$1 \le N \le 2000$）和K（$0 \le K \le 10^{18}$）。

## 输出格式

只有一行，一个整数表示方案数。
因为答案可能会很大，所以请对$10^{9}+7$取模。

## 输入输出样例 #1

### 输入 #1

```
3 2
```

### 输出 #1

```
20
```

## 输入输出样例 #2

### 输入 #2

```
2 99
```

### 输出 #2

```
9900
```

## 输入输出样例 #3

### 输入 #3

```
3 5
```

### 输出 #3

```
188
```

## 输入输出样例 #4

### 输入 #4

```
7 20
```

### 输出 #4

```
744195543
```