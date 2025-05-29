## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc118/tasks/arc118_a

ARC 国の消費税率は $ t $ パーセントです。ただし $ t $ は正の整数です。

ARC 国には整数屋さんがあります。整数屋さんでは各正の整数 $ A $ を税抜き価格 $ A $ 円で取り扱っており、その税込み価格は $ \left\lfloor\frac{100+t}{100}A\right\rfloor $ 円です。ただし実数 $ x $ に対し、$ \lfloor\ x\rfloor $ は $ x $ 以下の最大の整数を表します。

あらゆる正の整数を取り扱っている整数屋さんですが、その税込み価格としては現れない正の整数の金額が存在します。そのような金額のうち、小さい方から $ N $ 番目のものを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ t $ $ N $

## 输出格式
答えを出力してください。

```input1
10 1
```

```output1
10
```

```input2
3 5
```

```output2
171
```

```input3
1 1000000000
```

```output3
100999999999
```

## 提示
### 制約

- $ 1\leq\ t\leq\ 50 $
- $ 1\leq\ N\leq\ 10^{9} $

### Sample Explanation 1

この例では、消費税率は $ 10 $ パーセントです。 - 整数 $ 9 $ の税込み価格は $ \left\lfloor\ \frac{110}{100}\times\ 9\right\rfloor\ =\ \lfloor\ 9.9\rfloor\ =\ 9 $ 円です。 - 整数 $ 10 $ の税込み価格は $ \left\lfloor\ \frac{110}{100}\times\ 10\right\rfloor\ =\ \lfloor\ 11\rfloor\ =\ 11 $ 円です。 これらから、$ 10 $ 円という金額は税込み価格として現れないことが分かります。この金額が、税込み価格として現れない最小の金額となります。

### Sample Explanation 2

消費税率が $ 3 $ パーセントの場合、税込み価格として現れない金額は、小さい方から順に $ 34,\ 68,\ 102,\ 137,\ 171,\ \ldots $ となります。

