# AT_pakencamp_2021_day2_k Bracket Inserting

## 题目描述

龟君对字符串玩法情有独钟。今天，他开始了一个有趣的游戏，从一个空字符串 $ s $ 开始，他进行了以下操作 $ N $ 次：

- 把 $ s $ 分成两个字符串 $ l $ 和 $ r $。然后用 $ l\ + $ `()` $ +\ r $ 替换 $ s $。

现在，给你 $ N $ 次操作完成后的字符串 $ s $，即 $ T $，你的任务是找出所有可能的操作方法的数量，并将其对 $ 998244353 $ 取模后输出。

需要注意的是，如果存在一个正整数 $ k\ (1\ \le\ k\ \le\ N) $，使得第 $ k $ 次操作中的 $ (l, r) $ 不同，那么这两种操作方法被认为是不同的。

另外，考虑到龟君一定是诚实的，给定的字符串 $ T $ 总能通过某种合法的操作方法获得。

## 输入格式

标准输入给出如下格式：

> $ N $ $ T $

## 输出格式

输出结果。

## 输入输出样例 #1

### 输入 #1

```
3
(())()
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
1
()
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
7
(()(()(())()))
```

### 输出 #3

```
72
```

## 说明/提示

### 约束

- $ 1\ \le\ N\ \le\ 10^5 $
- $ T $ 是由 `(` 和 `)` 组成的长度为 $ 2N $ 的字符串
- 通过合适的操作，总是可以使 $ s=T $

### 样例解释 1

考虑一种可能的操作：第一次操作时，$ l $ 和 $ r $ 为空字符串，所以 $ s= $ `()`；第二次操作时，令 $ l= $ `()`，$ r $ 为空字符串，于是 $ s= $ `()()`；第三次操作时，选择 $ l= $ `(`，$ r= $ ` )()`，于是 $ s= $ `(())()`。

### 样例解释 3

出题者：\[turtle0123\_\_\](https://atcoder.jp/users/turtle0123\_\_)

 **本翻译由 AI 自动生成**