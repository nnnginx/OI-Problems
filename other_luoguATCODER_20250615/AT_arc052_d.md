# AT_arc052_d [ARC052D] 9

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc052/tasks/arc052_d

整数の $ 9 $ には面白い性質があります。 どのような非負整数 $ N $ を選んでも $ N $ を $ 9 $ で割った余りと、 $ N $ を $ 10 $ 進法で表記した時の各桁の数字の和を $ 9 $ で割った余りが一致するのです。

高橋君はこのような性質を持つ整数が他にないか気になりました。しかし、残念なことにこのような性質をもつ整数は $ 9 $ と $ 3 $ と $ 1 $ くらいしか見つかりませんでした。 そこで、「どのような非負整数 $ N $ を選んでも・・・」ではなくて「できるだけ多くの非負整数 $ N $ に対して・・・」というふうに性質の条件を落として探してみることにしてみました。

高橋君は非負整数 $ K $ がどれくらい多くの非負整数 $ N $ に対して上のような条件をみたすのかが知りたいです。

高橋君を手伝うために以下の問いに答えてください。

- $ 1\ ≦\ N\ ≦\ M $ となる整数 $ N $ のうち $ K $ で割った余りと、$ N $ を $ 10 $ 進法表記した時の各桁の数字の和を $ K $ で割った余りが一致するような $ N $ の個数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ K $ $ M $

## 输出格式

問題文で挙げた条件に一致する非負整数の個数を $ 1 $ 行で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 100
```

### 输出 #1

```
19
```

## 输入输出样例 #2

### 输入 #2

```
112 32279
```

### 输出 #2

```
309
```

## 输入输出样例 #3

### 输入 #3

```
108 3141592653
```

### 输出 #3

```
261799999
```

## 输入输出样例 #4

### 输入 #4

```
9 10000000000
```

### 输出 #4

```
10000000000
```

## 说明/提示

### 制約

- 与えられる数字はすべて整数
- $ 1\ ≦\ K\ ≦\ M\ ≦\ 10^{10} $

### 部分点

この問題には部分点が設定されている。

- $ 1\ ≦\ M\ ≦\ 10^5 $ を満たすデータセットに正解した場合は $ 10 $ 点が与えられる。
- $ 1\ ≦\ M\ ≦\ 10^{10} $を満たすデータセットに正解した場合はさらに $ 90 $ 点が与えられる。合計で$ 100 $点となる。

### Sample Explanation 1

$ 1 $桁の整数はかならず条件を満たします。 そのほかに $ 50\ ≦\ N\ ≦\ 59 $ を満たす整数は全て条件を満たします。 これら以外に条件を満たす整数は $ 100 $ 以下の範囲にはありません。 よって $ 19 $ を出力します。