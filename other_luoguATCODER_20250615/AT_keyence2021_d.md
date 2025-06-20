# AT_keyence2021_d Choosing Up Sides

## 题目描述

[problemUrl]: https://atcoder.jp/contests/keyence2021/tasks/keyence2021_d

$ N $ を正の整数とします。 $ 2 $ つの $ 2^{N-1} $ 人チームが対戦する競技があります。

$ 1 $ から $ 2^N $ の番号がついた $ 2^N $ 人の人がいます。 すぬけ監督は、彼らを A と B の $ 2 $ つの $ 2^{N-1} $ 人チームに分けて対戦させる、という操作を何回でも行うことができます。

すぬけ監督は、$ 1 $ 回以上操作を行った後、以下の $ 2 $ つの条件の両方を満たすようにしたいです。

1. ある整数 $ n $ が存在して、$ 1\ \leq\ i\ <\ j\ \leq\ 2^N $ を満たす任意の $ (i,j) $ について、人 $ i $ と人 $ j $ が **同じ** チームだった回数が $ n $ 回
2. ある整数 $ m $ が存在して、$ 1\ \leq\ i\ <\ j\ \leq\ 2^N $ を満たす任意の $ (i,j) $ について、人 $ i $ と人 $ j $ が **異なる** チームだった回数が $ m $ 回

すぬけ監督の要望を満たすような操作列が存在することが証明できます。そのうち **操作回数が最小** であるようなものの一例を示してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

下記のフォーマットで操作列を出力せよ。

> $ K $ $ s_1 $ $ s_2 $ $ \vdots $ $ s_K $

ここで、$ K $ は操作列の長さを、$ s_i $ は $ i $ 回目の操作でのチーム分けを表す。 $ s_{i} $ は長さ $ 2^N $ の `A`, `B` のみからなる文字列であり、$ s_{i} $ の $ {j} $ 文字目が `A` ならば $ i $ 回目の操作で人 $ j $ はチーム A に所属していたことを、`B` ならばチーム B に所属していたことを表す。`A`, `B` は $ s_i $ において $ 2^{N-1} $ 回ずつ出現する必要があることに注意せよ。

$ K $ が要望を満たす操作列の長さとして最小であり、操作の結果すぬけ監督の要望が満たされたならば正解となる。

## 输入输出样例 #1

### 输入 #1

```
1
```

### 输出 #1

```
1
AB
```

## 说明/提示

### 制約

- 与えられる入力は全て整数
- $ 1\ \leq\ N\ \leq\ 8 $

### Sample Explanation 1

\- $ 1 $ 回操作を行うことですぬけ監督の要望を満たすことができます。 - 操作は $ 1 $ 回以上行う必要があることに注意してください。