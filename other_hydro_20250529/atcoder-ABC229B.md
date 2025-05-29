## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc229/tasks/abc229_b

正整数 $ A,B $ が与えられます。  
 $ A+B $ を(十進法で)計算する時、繰り上がりが生じないなら `Easy` 、生じるなら `Hard` と出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $

## 输出格式
繰り上がりが生じないなら `Easy` 、生じるなら `Hard` と出力せよ。

## 题目大意
给定两个正整数 $a,b$ ，如果计算 $a+b$ 时发生了进位输出 `Hard` ，否则输出 `Easy` 。注意， $a,b≤10^{18}$ 。

```input1
229 390
```

```output1
Hard
```

```input2
123456789 9876543210
```

```output2
Easy
```

## 提示
### 制約

- $ A,B $ は整数
- $ 1\ \le\ A,B\ \le\ 10^{18} $

### Sample Explanation 1

$ 229+390 $ を計算する際、十の位から百の位へと繰り上がりが発生します。よって、答えは `Hard` です。

### Sample Explanation 2

繰り上がりは発生しません。答えは `Easy` です。 また、入力が $ 32 $bit 整数に収まらないこともあります。

