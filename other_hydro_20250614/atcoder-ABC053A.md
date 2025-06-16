## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc053/tasks/abc053_a

すめけくんは現在のレートが $ 1200 $ 未満ならば AtCoder Beginner Contest (ABC) に、そうでなければ AtCoder Regular Contest (ARC) に参加することにしました。 すめけくんの現在のレート $ x $ が与えられます。すめけくんが参加するコンテストが ABC ならば `ABC` と、そうでなければ `ARC` と出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ x $

## 输出格式
答えを出力せよ。

## 题目大意
输入一个整数 $x$ ， 如果 $x$ 小于 $1200$ ，那么输出 ```ABC``` ，否则输出 ```ARC ``` 。

```input1
1000
```

```output1
ABC
```

```input2
2000
```

```output2
ARC
```

## 提示
### 制約

- $ 1\ ≦\ x\ ≦\ 3{,}000 $
- $ x $ は整数

### Sample Explanation 1

すめけくんの現在のレートは $ 1200 $ 未満なので `ABC` と出力してください。

### Sample Explanation 2

すめけくんの現在のレートは $ 1200 $ 以上なので `ARC` と出力してください。

