## 题目描述

ftiasch 是个十分受女生欢迎的同学，所以她总是收到许多情书。虽然她十分有魅力，然而她却是个低调的人。因此她从来不会告诉别人她到底收到了多少情书。

ftiasch 的好朋友 1tthinking 想知道她到底收到了多少情书。1tthinking 知道，ftiasch 每次收到一封情书，就会在日记最后写下一个包含 `luvletter` 子序列的串。比如现在 ftiasch 的日记是 `alduddvdletterflusvletetedr`，那么 ftiasch 可能收到了 $0,1,2$ 封情书。

现在给出一些 ftiasch 的日记，问对于每篇日记，ftiasch 最多可能受到多少的情书。

## 输入格式

第一行一个整数 $T$ 表示数据组数。

接下来 $T$ 行，每行一个串表示一篇日记 $s$，保证只包含小写字母以及空格。

## 输出格式

共 $T$ 行，每行一个整数表示对应询问的答案。

```input1
5
t
llllluvletterrr
luvletterlauavalaeatataearaluvletter
is wzk a famous boy yes buz he always receives a lot of luv letters
my heart beats her waves at the shore of the world and writes upon it her signature in tears with the words i love thee
```

```output1
0
1
3
1
0
```

## 数据规模与约定

对于 $100\%$ 的数据，$0\leq T\leq 100$，$1\leq|s|\leq 10^5$。

