# AT_codefestival_2016_qualA_c 次のアルファベット

## 题目描述

# 题意翻译
高桥君有一个仅由小写字母组成的字符串s。高桥君对s执行以下操作正好是k次。在所需位置从字符串s中选择一个字母并将该字母更改为下一个字母。但是,z后面的字母是a。例如，如果选择字符串aaz的第2个字符并执行操作aaz → abz。 然后，如果选择abz的 第3个字符并执行操作，则它变为aba。高桥君 希望在k操作后，按字典顺序使字符串s尽可能小。仅在k次操作后，按字典顺序输出最小的字符串s。

## 输入格式

第一行一个字符串s，第二行一个整数k。

## 输出格式

k次操作后字典顺序最小的字符串s.
# 输入输出样例
## 输入#1
xyz          
4
## 输出#1
aya
## 输入#2
a   
25
## 输出#2
z
## 输入#3
codefestival   
100
## 输出#3
aaaafeaaivap

## 输入输出样例 #1

### 输入 #1

```
xyz
4
```

### 输出 #1

```
aya
```

## 输入输出样例 #2

### 输入 #2

```
a
25
```

### 输出 #2

```
z
```

## 输入输出样例 #3

### 输入 #3

```
codefestival
100
```

### 输出 #3

```
aaaafeaaivap
```

## 说明/提示

设字符串s的长度为n  
+ 1≤n≤100000
+ 1≤k≤1000000000