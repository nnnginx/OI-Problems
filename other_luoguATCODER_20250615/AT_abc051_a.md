# AT_abc051_a [ABC051A] Haiku

## 题目描述

海豚在新年收到了长度为 $19$ 的字符串 $s$。
其格式由 $5$ 个小写字母、$7$ 个小写字母和 $5$ 个小写字母表示，中间由 **逗号** 分隔开。

海豚希望将由 **逗号** 分隔的字符串 $s$ 转换为由 **空格** 分隔的字符串。
请你帮海豚制作一个用于处理的程序。

## 输入格式

输入一个字符串 $s$。由标准输入给出。

## 输出格式

输出处理后的字符串 $s$。

## 输入输出样例 #1

### 输入 #1

```
happy,newyear,enjoy
```

### 输出 #1

```
happy newyear enjoy
```

## 输入输出样例 #2

### 输入 #2

```
haiku,atcoder,tasks
```

### 输出 #2

```
haiku atcoder tasks
```

## 输入输出样例 #3

### 输入 #3

```
abcde,fghihgf,edcba
```

### 输出 #3

```
abcde fghihgf edcba
```

## 说明/提示

#### 数据规模与约定
对于 $100\%$ 的测试点数据，保证：
- $\lvert s\rvert=19$。
- $s_6$ 和 $s_{14}$ 均为 `,`（下标从 $1$ 开始）。
- 其余字符均为小写字母。

#### 样例 $1$ 解释
用空格替换 `happy,newyear,enjoy` 中的所有逗号，输出 `happy newyear enjoy`。

---
翻译：@[Wuzetong](https://www.luogu.com.cn/user/1219873)