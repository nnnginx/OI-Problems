## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc068/tasks/arc068_c

すぬけくんは鉄道会社を運営するゲームで遊ぶことにしました。すぬけ鉄道には $ M+1 $ 個の駅があり、 $ 0 $ から $ M $ までの番号がついています。 すぬけ鉄道の列車は駅 $ 0 $ から $ d $ 駅ごとに停車します。 例えば $ d\ =\ 3 $ のとき駅 $ 0 $,駅 $ 3 $,駅 $ 6 $,駅 $ 9 $, $ ... $ に停車します。

すぬけ鉄道が走っている地域には $ N $ 種類の名産品があり、種類 $ i $ の名産品は 駅 $ l_i $,駅 $ l_i+1 $,駅 $ l_i+2 $, $ ... $, 駅 $ r_i $ のいずれかに列車が停車したとき購入することが可能です。

列車が停車する間隔 $ d $ は $ 1,\ 2,\ 3,\ ...,\ M $ の $ M $ 種類が存在しています。 $ M $ 種類の列車それぞれについて、その列車に駅 $ 0 $ で乗車した場合に購入可能な名産品の種類数を求めなさい。 なお、列車から別の列車への乗り換えは許されないものとします。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ l_1 $ $ r_1 $ $ : $ $ l_{N} $ $ r_{N} $

## 输出格式
答えを $ M $ 行に出力せよ。 $ i $ 行目では $ i $ 駅ごとに停車する列車に乗った場合に購入可能な名産品の種類数を出力せよ。

## 题目大意
有一趟列车有 $M+1$ 个车站，从 $0$ 到 $M$ 编号。有 $N$ 种商品，第 $i$ 种只在编号 $[l_i,r_i]$ 的车站出售。一辆列车有一个预设好的系数 $d$，从 $0$ 出发，只会在 $d$ 的倍数车站停车。对于 $d$ 从 $1$ 到 $M$ 的列车，求最多能买到多少种商品。

```input1
3 3
1 2
2 3
3 3
```

```output1
3
2
2
```

```input2
7 9
1 7
5 9
5 7
5 9
1 1
6 8
3 4
```

```output2
7
6
6
5
4
5
5
3
2
```

## 提示
### 制約

- $ 1\ ≦\ N\ ≦\ 3\ ×\ 10^{5} $
- $ 1\ ≦\ M\ ≦\ 10^{5} $
- $ 1\ ≦\ l_i\ ≦\ r_i\ ≦\ M $

### Sample Explanation 1

\- $ 1 $ 駅ごとに停車する列車に乗った場合、種類 $ 1,2,3 $ の $ 3 $ 種類の名産品を購入することが可能です。 - $ 2 $ 駅ごとに停車する列車に乗った場合、種類 $ 1,2 $ の $ 2 $ 種類の名産品を購入することが可能です。 - $ 3 $ 駅ごとに停車する列車に乗った場合、種類 $ 2,3 $ の $ 2 $ 種類の名産品を購入することが可能です。

