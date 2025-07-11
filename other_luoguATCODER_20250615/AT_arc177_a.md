# AT_arc177_a [ARC177A] Exchange

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc177/tasks/arc177_a

日本では、$ 1 $ 円、$ 5 $ 円、$ 10 $ 円、$ 50 $ 円、$ 100 $ 円、$ 500 $ 円の $ 6 $ 種類の硬貨が流通しています。これについて、次の問いに答えてください。

> AtCoder さんの財布の中には、$ 1 $ 円硬貨 $ A $ 枚、$ 5 $ 円硬貨 $ B $ 枚、$ 10 $ 円硬貨 $ C $ 枚、$ 50 $ 円硬貨 $ D $ 枚、$ 100 $ 円硬貨 $ E $ 枚、$ 500 $ 円硬貨 $ F $ 枚が入っています。
> 
> AtCoder さんは、これから $ N $ 個の店で順番に買い物を行います。 具体的には、$ i $ 番目 $ (1\ \leq\ i\ \leq\ N) $ に訪れる店では税込 $ X_i $ 円の商品を $ 1 $ つ購入する予定です。
> 
> 釣銭の授受には時間がかかるので、彼は支払いに使う硬貨を上手く選ぶことで、すべての店で**ちょうどの金額**を支払って商品を購入したいです。 このようなことが可能か、判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられます。

> $ A $ $ B $ $ C $ $ D $ $ E $ $ F $ $ N $ $ X_1 $ $ X_2 $ $ \cdots $ $ X_N $

## 输出格式

可能ならば `Yes`、不可能ならば `No` と出力してください。

## 输入输出样例 #1

### 输入 #1

```
0 0 6 3 4 1
3
700 250 160
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
0 0 0 2 4 0
3
100 200 300
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
0 0 0 0 8 8
1
250
```

### 输出 #3

```
No
```

## 输入输出样例 #4

### 输入 #4

```
20 5 9 7 10 6
5
177 177 177 177 177
```

### 输出 #4

```
Yes
```

## 输入输出样例 #5

### 输入 #5

```
17 5 9 7 10 6
5
177 177 177 177 177
```

### 输出 #5

```
No
```

## 说明/提示

### 制約

- $ 0\ \leq\ A\ \leq\ 200 $
- $ 0\ \leq\ B\ \leq\ 200 $
- $ 0\ \leq\ C\ \leq\ 200 $
- $ 0\ \leq\ D\ \leq\ 200 $
- $ 0\ \leq\ E\ \leq\ 200 $
- $ 0\ \leq\ F\ \leq\ 200 $
- $ 1\ \leq\ N\ \leq\ 10 $
- $ 1\ \leq\ X_i\ \leq\ 10000\ (1\ \leq\ i\ \leq\ N) $
- 入力はすべて整数
 
### Sample Explanation 1

たとえば以下のように支払いを行うと、$ 3 $ 店舗すべてでちょうどの支払いを行うことができます。 - $ 1 $ 番目に訪れる店：$ 100 $ 円硬貨を $ 2 $ 枚、$ 500 $ 円硬貨を $ 1 $ 枚使う。 - $ 2 $ 番目に訪れる店：$ 10 $ 円硬貨を $ 5 $ 枚、$ 100 $ 円硬貨を $ 2 $ 枚使う。 - $ 3 $ 番目に訪れる店：$ 10 $ 円硬貨を $ 1 $ 枚、$ 50 $ 円硬貨を $ 3 $ 枚使う。

### Sample Explanation 2

財布に入っている金額は $ 500 $ 円ですが、合計 $ 100+200+300=600 $ 円の支払いを行う必要があるため、すべての商品を購入することができません。

### Sample Explanation 3

財布に $ 50 $ 円以下の硬貨が入っていないため、$ 250 $ 円ちょうどを支払うことはできません。