# AT_abc297_b [ABC297B] chess960

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc297/tasks/abc297_b

> 高橋君は chess960 と呼ばれるゲームで遊んでいます。 高橋君はランダムに決めた初期配置が chess960 の条件を満たすか確認するプログラムを書くことにしました。

長さ $ 8 $ の文字列 $ S $ が与えられます。$ S $ には `K`, `Q` がちょうど $ 1 $ 文字ずつ、`R`, `B`, `N` がちょうど $ 2 $ 文字ずつ含まれます。 $ S $ が以下の条件を全て満たしているか判定してください。

- $ S $ において左から $ x,y\ (x\ <\ y) $ 文字目が `B` であるとする。このとき $ x $ と $ y $ の偶奇が異なる。
- `K` は $ 2 $ つの `R` の間にある。より形式的には、$ S $ において左から $ x,y\ (x\ <\ y) $ 文字目が `R` であり、 $ z $ 文字目が `K` であるとする。このとき、 $ x\ <\ z\ <\ y $ が成り立つ。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

$ S $ が条件を満たす場合 `Yes` を、そうでない場合 `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
RNBQKBNR
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
KRRBBNNQ
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
BRKRBQNN
```

### 输出 #3

```
No
```

## 说明/提示

### 制約

- $ S $ は 長さ $ 8 $ の文字列であり、`K`, `Q` がちょうど $ 1 $ 文字ずつ、`R`, `B`, `N` がちょうど $ 2 $ 文字ずつ含まれる。
 
### Sample Explanation 1

`B` は左から $ 3 $ 番目、$ 6 $ 番目にあり、$ 3 $ と $ 6 $ は偶奇が異なります。 また、`K` は $ 2 $ つの `R` の間にあります。よって条件を満たします。

### Sample Explanation 2

`K` は $ 2 $ つの `R` の間にありません。