# AT_icpc2015summer_day2_c ABC Gene

## 题目描述

用一个字符串 `ABC` 来表示基因序列，你可以通过进行若干次下述操作来改变这个基因序列：

* 从 `A`，`B`，`C` 三个字母中选出一个，记作 $x$，将字符串中所有的 $x$ 替换为 `ABC`。

现在给出另一个由 `A`，`B`，`C` 组成的基因序列 $S$，问能否将基因序列 `ABC` 通过若干次上述操作变为 $S$。

## 输入格式

输入来自以下格式的标准输入：

---

$S$

---

## 输出格式

如果能将 `ABC` 通过若干次上述操作得到基因序列 $S$，输出 `Yes`，否则输出 `No`。

### 输入输出样例

**输入 #1**

```plain
ABC
```

**输出 #1**

```plain
Yes
```

基因序列本身就是 `ABC`。

**输入 #2**

```plain
AABCC
```

**输出 #2**

```plain2
Yes
```

选择 `B` 进行操作，`ABC`$\rightarrow$`AABCC`。

**输入 #3**

```plain
AABCABC
```

**输出 #3**

```plain
No
```

如果选择 `C` 进行操作，也不会使 `AABCC`$\rightarrow$`AABCABC`。事实上，由于所有 `C` 都要进行替换，所以该操作会使 `AABCC`$\rightarrow$`AABABCABC`。

## 说明/提示

* $1 \le |S| \le 5\times 10^3$。

* $S$ 只包含 `A`，`B`，`C` 三种字符。