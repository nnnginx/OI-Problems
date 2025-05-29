## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc212/tasks/abc212_a

高橋くんは $ A $ グラムの純金と $ B $ グラムの純銀 $ (0\ \leq\ A,B,\ 0\ \lt\ A+B) $ をよく溶かした上で混ぜ合わせ、新たな金属を生成しました。

生成された金属は「純金」「純銀」「合金」のいずれでしょうか？

なお、生成された金属は

- $ 0\ \lt\ A $ かつ $ B=0 $ なら「純金」
- $ A=0 $ かつ $ 0\ \lt\ B $ なら「純銀」
- $ 0\ \lt\ A $ かつ $ 0\ \lt\ B $ なら「合金」

であるとみなします。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $

## 输出格式
生成された金属が「純金」なら `Gold` と、「純銀」なら `Silver` と、「合金」なら `Alloy` と出力せよ。

## 题目大意
输入两个非负整数 $a,b$ ，如果 $a=0$ 输出“Silver”，如果 $b=0$ 输出“Gold”，如果 $a,b$ 都大于 $0$ 输出“Alloy”。（注：输出时的字符串不含双引号）

```input1
50 50
```

```output1
Alloy
```

```input2
100 0
```

```output2
Gold
```

```input3
0 100
```

```output3
Silver
```

```input4
100 2
```

```output4
Alloy
```

## 提示
### 制約

- $ 0\ \leq\ A,B\ \leq\ 100 $
- $ 0\ \lt\ A+B $
- $ A,B $ は整数

### Sample Explanation 1

$ 0\ \lt\ A $ かつ $ 0\ \lt\ B $ であるため、生成された金属は「合金」です。

### Sample Explanation 2

$ 0\ \lt\ A $ かつ $ B=0 $ であるため、生成された金属は「純金」です。

### Sample Explanation 3

$ A=0 $ かつ $ 0\ \lt\ B $ であるため、生成された金属は「純銀」です。

