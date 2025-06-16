## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc115/tasks/abc115_a

とある世界では、今日は $ 12 $ 月 $ D $ 日です。

$ D\ =\ 25 $ なら `Christmas`, $ D\ =\ 24 $ なら `Christmas Eve`, $ D\ =\ 23 $ なら `Christmas Eve Eve`, $ D\ =\ 22 $ なら `Christmas Eve Eve Eve` と出力するプログラムを作ってください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ D $

## 输出格式
指定された文字列を出力せよ (大文字と小文字は区別される)。

## 题目大意
今天是$12$月$d$日。

请你编写程序，如果$d=25$，输出`Christmas`；如果$d=24$，输出`Christmas Eve`；如果$d=23$，输出`Christmas Eve Eve`；如果$d=22$，输出`Christmas Eve Eve Eve`。

```input1
25
```

```output1
Christmas
```

```input2
22
```

```output2
Christmas Eve Eve Eve
```

## 提示
### 制約

- $ 22\ \leq\ D\ \leq\ 25 $
- $ D $ は整数である。

### Sample Explanation 2

単語と単語の間のスペースも出力してください。

