# AT_abc143_c [ABC143C] Slimes

## 题目描述

【问题描述】

有$N$个史莱姆从左到右排列。这些史莱姆的颜色将以只由小写英文字母的字符串$S$给出。第$i$个史莱姆的颜色是字符串$S$的第$i$位。

具有相同颜色的相邻的史莱姆将融合为一个更大的史莱姆，而不会更改颜色。如果在融合之前这组史莱姆旁边有其他史莱姆，那么旁边的史莱姆现在就与新的更大的史莱姆相邻。

最终，会有多少史莱姆？

## 输入格式

输入第一行一个整数$N$，表示史莱姆的个数。

第二行一个字符串$S$，表示史莱姆的颜色。

## 输出格式

输出一个整数，表示最终会有多少史莱姆。

## 输入输出样例 #1

### 输入 #1

```
10
aabbbbaaca
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
5
aaaaa
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
20
xxzaffeeeeddfkkkkllq
```

### 输出 #3

```
10
```

## 说明/提示

样例$1$：最终，这些史莱姆将融合为`abaca`。

样例$2$：所有的史莱姆将融合为一个。

【数据规模与约定】

对于$100%$的数据，$1\leq N\leq 10^5，|S|=N$。

感谢@[Celtic](https://www.luogu.com.cn/user/176990)提供的翻译。