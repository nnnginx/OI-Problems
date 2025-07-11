# AT_arc068_b [ABC053D] Card Eater

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc053/tasks/arc068_b

すぬけくんはカードゲームで遊ぶことにしました。 $ N $ 枚からなるカードの山があり、上から $ i $ 枚目のカードには整数 $ A_i $ が書かれています。

すぬけくんはこのカードの山に対し $ 0 $ 回以上、以下の操作を行い、残ったカードに書かれた値が互いに異なるようにしたいです。最大で何枚のカードを残すことが可能か求めなさい。なお、$ N $ は奇数であり、少なくとも $ 1 $ 枚のカードを残すことが可能であることが保証されます。

操作：カードの山から任意の $ 3 $ 枚のカードを抜き出す。抜き出したカードのうち書かれた値が最大であるようなカード $ 1 $ 枚と最小であるようなカード $ 1 $ 枚の合計 $ 2 $ 枚を選んで食べる。その後残った $ 1 $ 枚をカードの山に戻す。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ A_3 $ ... $ A_{N} $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
1 2 1 3 7
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
15
1 3 5 2 1 3 2 8 8 6 2 6 11 1 1
```

### 输出 #2

```
7
```

## 说明/提示

### 制約

- $ 3\ ≦\ N\ ≦\ 10^{5} $
- $ N $ は奇数
- $ 1\ ≦\ A_i\ ≦\ 10^{5} $
- $ A_i $ は整数

### Sample Explanation 1

操作を $ 1 $ 回行って $ 1,1,2 $ を取り出すというのが最適な操作手順の $ 1 $ つです。最大値である $ 2 $ と書かれたカードで最小値である $ 1 $ と書かれたカードがそれぞれ $ 1 $ 枚ずつ食べられ、残った $ 1 $ と書かれたカードがカードの山に戻されます。カードの山に残っているカードは $ 1,3,7 $ となり、これらは互いに異なります。