# AT_cf16_exhibition_final_g FESTIVAL

## 题目描述

[problemUrl]: https://atcoder.jp/contests/cf16-exhibition-final/tasks/cf16_exhibition_final_g

CODE FESTIVAL 2016 へようこそ! このコンテストを祝うために、以下の条件を満たす文字列 $ s $ を一つ見つけてください：

- $ s $ の長さは $ 1 $ 以上 $ 5000 $ 以下である。
- $ s $ は英大文字のみからなる。
- $ s $ は文字列 "FESTIVAL" をちょうど $ K $ 回部分列として含む。 言い換えると、 $ 0\ <\ =\ i_0\ <\ i_1\ <\ ...\ <\ i_7\ <\ =\ |s|-1 $ かつ $ s[i_0]='F',\ s[i_1]='E',\ ...,\ s[i_7]='L' $ を満たすような組 $ (i_0,\ i_1,\ ...,\ i_7) $ がちょうど $ K $ 組存在する。

与えられた制約の元では、必ず解が存在することが証明できます。 複数通りの解が考えられる場合は、どれを出力してもかまいません。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ K $

## 输出格式

条件を満たす文字列を一つ出力せよ。

## 输入输出样例 #1

### 输入 #1

```
7
```

### 输出 #1

```
FESSSSSSSTIVAL
```

## 输入输出样例 #2

### 输入 #2

```
256
```

### 输出 #2

```
FFEESSTTIIVVAALL
```

## 说明/提示

### 制約

- $ 1\ <\ =\ K\ <\ =\ 10^{18} $