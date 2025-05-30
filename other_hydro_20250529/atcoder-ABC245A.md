## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc245/tasks/abc245_a

ある日、高橋君は $ A $ 時 $ B $ 分ちょうどに、青木君は $ C $ 時 $ D $ 分 $ 1 $ 秒に起きました。  
 高橋君の起床時刻が青木君より早いならば `Takahashi` を、そうでないならば `Aoki` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ D $

## 输出格式
高橋君の起床時刻が青木君より早いならば `Takahashi` を、そうでないならば `Aoki` を出力せよ。

## 题目大意
给定 $a,b,c,d$ ，求出 $a:b:00$ 和 $c:d:01$ 两个时刻中更早的时刻是哪个。若前者更早，输出Takahashi；否则输出Aoki。（保证输入的时间符合24小时制中的规定且输入均为整数）

```input1
7 0 6 30
```

```output1
Aoki
```

```input2
7 30 7 30
```

```output2
Takahashi
```

```input3
0 0 23 59
```

```output3
Takahashi
```

## 提示
### 制約

- $ 0\ \leq\ A\ \leq\ 23 $
- $ 0\ \leq\ B\ \leq\ 59 $
- $ 0\ \leq\ C\ \leq\ 23 $
- $ 0\ \leq\ D\ \leq\ 59 $
- 入力はすべて整数である。

### Sample Explanation 1

高橋君は $ 7 $ 時ちょうどに、青木君は $ 6 $ 時 $ 30 $ 分 $ 1 $ 秒に起きました。 青木君の起床時刻の方が早いため、`Aoki` を出力します。

### Sample Explanation 2

高橋君は $ 7 $ 時 $ 30 $ 分ちょうどに、青木君は $ 7 $ 時 $ 30 $ 分 $ 1 $ 秒に起きました。 高橋君の起床時刻の方が $ 1 $ 秒だけ早いため、`Takahashi` を出力します。

### Sample Explanation 3

ある日の $ 0 $ 時 $ 0 $ 分ちょうどはその日の $ 0 $ 時 $ 1 $ 分の $ 1 $ 分前であり、 その日の $ 23 $ 時 $ 59 $ 分の $ 1 $ 分後、すなわちいわゆる $ 24 $ 時ちょうどのことではありません。 よって、高橋君の起床時刻の方が早く、`Takahashi` を出力します。

