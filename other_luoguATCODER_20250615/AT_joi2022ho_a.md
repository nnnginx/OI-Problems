# AT_joi2022ho_a インターカステラー (Intercastellar)

## 题目描述

### 题目简述

有一条长度未知的线段，它被截成了若干段，从左往右数第 $i$ 段的长为 $a_i$。现在不断将长度为偶数的线段截成两条长度相等的线段（不改变线段位置），直至没有长度为偶数的线段。截完后，给出 $q$ 个询问，请按顺序回答每个询问。第 $i$ 个询问会输入一个整数 $x_i$，此时请输出左数第 $x_i$ 条线段的长度并换行。

## 输入格式

第一行：$n$

接下来 $n$ 行：第 $i$ 行为 $a_i$

接下来一行：$q$

接下来 $q$ 行：第 $i$ 行为 $x_i$

## 输出格式

输出 $q$ 行，第 $i$ 行输出的正整数为截完后左起第 $x_i$ 条线段的长度。

## 输入输出样例 #1

### 输入 #1

```
4
14
9
8
12
6
2
3
5
7
11
13
```

### 输出 #1

```
7
9
1
1
1
3
```

## 输入输出样例 #2

### 输入 #2

```
13
1
4
1
4
2
1
3
5
6
2
3
7
3
8
2
10
11
13
15
17
18
20
```

### 输出 #2

```
1
1
1
1
5
3
1
3
```

## 输入输出样例 #3

### 输入 #3

```
16
536870912
402653184
536870912
536870912
134217728
536870912
671088640
536870912
536870912
536870912
939524096
805306368
536870912
956301312
536870912
536870912
5
2500000000
3355443201
4294967296
5111111111
6190792704
```

### 输出 #3

```
5
1
7
57
1
```