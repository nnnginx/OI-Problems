# AT_abc019_2 [ABC019B] 高橋くんと文字列圧縮

## 题目描述

将字符串经过以下步骤压缩后输出：

1. 将字符串$s$按照连续字符分割成若干个子串。
2. 将每个子串里的字符和子串的长度链接起来，形成新的子串。
3. 将若干个新的子串连接起来，形成新的字符串。

例如：字符串`aabbbaad`的压缩过程：

1. 将`aabbbaad`分割成`aa``bbb``aa``d`;
2. 将`aa``bbb``aa``d`转换成`a2``b3``a2``d1`;
3. 将`a2``b3``a2``d1`链接起来形成`a2b3a2d1`。

`a2b3a2d1`就是压缩后的字符串。

## 输入格式

输入按照以下格式：
```
$ s $
```

- $1 \leq s$的长度$ \leq 1,000$
- 保证$s$是由英文小写字母组成。

## 输出格式

输出$s$被压缩后的字符串。

输出末尾需换行。

## 输入输出样例 #1

### 输入 #1

```
aabbbaad
```

### 输出 #1

```
a2b3a2d1
```

## 输入输出样例 #2

### 输入 #2

```
aabbbbbbbbbbbbxyza
```

### 输出 #2

```
a2b12x1y1z1a1
```

## 输入输出样例 #3

### 输入 #3

```
edcba
```

### 输出 #3

```
e1d1c1b1a1
```