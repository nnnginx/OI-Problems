# AT_abc352_g [ABC352G] Socks 3

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc352/tasks/abc352_g

高橋君のタンスの中には様々な色の靴下が入っています。 靴下の色は $ 1 $ 以上 $ N $ 以下の整数として表され、色 $ i $ の靴下は $ A_i\ (\geq\ 2) $ 枚入っています。

高橋君は、以下の操作を行うことで今日履く靴下を選ぼうとしています。

- 今までに取り出した靴下の中で同じ色の靴下の $ 2 $ 枚組が作れるようになるまで、タンスの中からランダムに等確率で $ 1 $ 枚の靴下を取り出すことを繰り返す。 なお、一度取り出した靴下はタンスの中には戻さない。

高橋君がタンスから靴下を取り出す回数の期待値を $ \text{mod\ }\ 998244353 $ で求めてください。

期待値を $ \text{mod\ }\ 998244353 $ で求めるとは求める期待値は必ず有理数になることが証明できます。 また、この問題の制約下では、期待値を既約分数 $ \frac{y}{x} $ で表したときに $ x $ が $ 998244353 $ で割り切れないことが保証されます。 このとき $ xz\ \equiv\ y\ \pmod{998244353} $ を満たすような $ 0 $ 以上 $ 998244352 $ 以下の整数 $ z $ が一意に定まるので、この $ z $ を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
2 2
```

### 输出 #1

```
665496238
```

## 输入输出样例 #2

### 输入 #2

```
1
352
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
6
1796 905 2768 253 2713 1448
```

### 输出 #3

```
887165507
```

## 说明/提示

### 制約

- $ 1\leq\ N\ \leq\ 3\times\ 10^5 $
- $ 2\leq\ A_i\ \leq\ 3000 $
- 入力は全て整数

### Sample Explanation 1

例えば、以下のように操作を行うことが考えられます。 1. タンスの中から色 $ 1 $ の靴下を $ 1 $ 枚取り出す。タンスの中には色 $ 1 $ の靴下が $ 1 $ 枚と色 $ 2 $ の靴下が $ 2 $ 枚残っている。 2. タンスの中から色 $ 2 $ の靴下を $ 1 $ 枚取り出す。タンスの中には色 $ 1,2 $ の靴下が $ 1 $ 枚ずつ残っている。 3. タンスの中から色 $ 1 $ の靴下を $ 1 $ 枚取り出す。今までに取り出した靴下は色 $ 1 $ の靴下が $ 2 $ 枚と色 $ 2 $ の靴下が $ 1 $ 枚であり、この中で色 $ 1 $ の靴下の $ 2 $ 枚組が作れるので操作を終了する。 この例の場合、高橋君がタンスから靴下を取り出す回数は $ 3 $ 回です。 高橋君がタンスから靴下を取り出す回数は $ \frac{2}{3} $ の確率で $ 3 $ 回、$ \frac{1}{3} $ の確率で $ 2 $ 回なので、求める期待値は $ 3\times\ \frac{2}{3}\ +\ 2\times\ \frac{1}{3}\ =\ \frac{8}{3}\ \equiv\ 665496238\ \pmod\ {998244353} $ です。