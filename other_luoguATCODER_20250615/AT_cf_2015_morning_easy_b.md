# AT_cf_2015_morning_easy_b ヘイホー君と置き換え

## 题目描述

**题意描述：**\
给定$1$个字符串$str$，要改动其中多少字符才可以使这个字符串重复呢？\
例子：
- 将第二个字符替换为 $a$，得 $aaacbabc$。
- 将第三个字符替换为 b，得 $aabcbabc$。
- 将第 5 个字符替换为 a，得 $aabcaabc$。\
这样重复的子串为$aabc$，符合题意。

## 输入格式

第一行为一个整数$N$$(1 ≦ N ≦ 100)$，表示字符串的长度。

第二行为初始字符串。

## 输出格式

修改此字符串的次数。

## 输入输出样例 #1

### 输入 #1

```
8
abacbabc
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
8
abababab
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
5
abcde
```

### 输出 #3

```
-1
```

## 输入输出样例 #4

### 输入 #4

```
26
codefestivaltwozeroonefive
```

### 输出 #4

```
11
```