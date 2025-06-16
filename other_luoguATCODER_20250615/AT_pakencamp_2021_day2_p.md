# AT_pakencamp_2021_day2_p A^k=k

## 题目描述

[problemUrl]: https://atcoder.jp/contests/pakencamp-2021-day2/tasks/pakencamp_2021_day2_p

$ T $ 個のケースについて、以下の問題を解いてください。

正整数 $ A,M $ が与えられます。 $ A^k\ \equiv\ k\ \pmod\ M $ を満たす非負整数 $ k\ (k\ <\ M\ \times\ \varphi\ (M)) $ の個数を求め($ ans $ とします)、条件を満たす $ k $ を $ \min(ans,1000) $ 個構築してください。

ただし、 $ \varphi(M) $ は[オイラーのファイ関数](https://ja.wikipedia.org/wiki/%E3%82%AA%E3%82%A4%E3%83%A9%E3%83%BC%E3%81%AE%CF%86%E9%96%A2%E6%95%B0)を表します。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ T $ $ \mathrm{case}_1 $ $ \mathrm{case}_2 $ $ \vdots $ $ \mathrm{case}_T $

各ケースは以下の形式で与えられる。

> $ A $ $ M $

## 输出格式

$ 2T $ 行出力せよ。 $ 2i-1 $ から $ 2i $ 行目には、 $ \mathrm{case}_i $ に対する答えを出力せよ。

各ケースについては、初めの行に問題文中で定義される $ ans $ を、次の行に空白区切りで条件を満たす $ k $ を $ \min(ans,1000) $ 個出力せよ。

ただし、出力する $ k $ はすべて相異なる必要がある。

## 输入输出样例 #1

### 输入 #1

```
1
2 4
```

### 输出 #1

```
1
4
```

## 说明/提示

### 制約

- $ 1\ \le\ T\ \le\ 100 $
- $ 1\ \leq\ A,M\ \leq\ 10^9 $
- 入力は全て整数

### Sample Explanation 1

$ 2^4\equiv\ 4\ \pmod\ 4 $ です。 原案: \[turtle0123\\\_\\\_\](https://atcoder.jp/users/turtle0123\_\_)