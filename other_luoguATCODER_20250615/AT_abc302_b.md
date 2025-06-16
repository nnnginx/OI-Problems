# AT_abc302_b [ABC302B] Find snuke

## 题目描述

给你一个 $H$ 行 $W$ 列的字符矩阵。请你在当中的行列或者 $45\degree$ 斜上的八个方向上寻找连续的五个字符 `s`，`n`，`u`，`k`，`e`，并依次输出它们的位置。保证有且仅有一组解。

## 输入格式

第一行 $2$ 个整数 $H,W$。

接下来 $H$ 行每行一个长度为 $W$ 的字符串。

## 输出格式

共五行，每行两个整数，依次表示找到的 `s`，`n`，`u`，`k`，`e` 的坐标。

## 输入输出样例 #1

### 输入 #1

```
6 6
vgxgpu
amkxks
zhkbpp
hykink
esnuke
zplvfj
```

### 输出 #1

```
5 2
5 3
5 4
5 5
5 6
```

## 输入输出样例 #2

### 输入 #2

```
5 5
ezzzz
zkzzz
ezuzs
zzznz
zzzzs
```

### 输出 #2

```
5 5
4 4
3 3
2 2
1 1
```

## 输入输出样例 #3

### 输入 #3

```
10 10
kseeusenuk
usesenesnn
kskekeeses
nesnusnkkn
snenuuenke
kukknkeuss
neunnennue
sknuessuku
nksneekknk
neeeuknenk
```

### 输出 #3

```
9 3
8 3
7 3
6 3
5 3
```