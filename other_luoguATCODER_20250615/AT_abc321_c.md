# AT_abc321_c [ABC321C] 321-like Searcher

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc321/tasks/abc321_c

以下の条件を満たす正整数 $ x $ を **321-like Number** と呼びます。 **この定義は A 問題と同様です。**

- $ x $ の各桁を上から見ると狭義単調減少になっている。
- すなわち、$ x $ が $ d $ 桁の整数だとすると、 $ 1\ \le\ i\ <\ d $ を満たす全ての整数 $ i $ について以下の条件を満たす。
  - ( $ x $ の上から $ i $ 桁目 ) $ > $ ( $ x $ の上から $ i+1 $ 桁目 )

なお、 $ 1 $ 桁の正整数は必ず 321-like Number であることに注意してください。

例えば、 $ 321,96410,1 $ は 321-like Number ですが、 $ 123,2109,86411 $ は 321-like Number ではありません。

$ K $ 番目に小さい 321-like Number を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ K $

## 输出格式

$ K $ 番目に小さい 321-like Number を整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
15
```

### 输出 #1

```
32
```

## 输入输出样例 #2

### 输入 #2

```
321
```

### 输出 #2

```
9610
```

## 输入输出样例 #3

### 输入 #3

```
777
```

### 输出 #3

```
983210
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ \le\ K $
- 321-like Number は $ K $ 個以上存在する

### Sample Explanation 1

321-like Number は小さいものから順に $ (1,2,3,4,5,6,7,8,9,10,20,21,30,31,32,40,\dots) $ です。 このうち $ 15 $ 番目に小さいものは $ 32 $ です。