## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc155/tasks/abc155_e

AtCoder 王国の通貨は $ 10^{100}+1 $ 種類の紙幣のみであり、価値はそれぞれ $ 1,\ 10,\ 10^2,\ 10^3,\ \dots,\ 10^{(10^{100})} $ です。あなたは商店街で、価値 $ N $ のたこ焼き器を $ 1 $ つ買おうとしています。

あなたは $ N $ 以上の金額を決めて支払います。その後、支払額よりちょうど $ N $ だけ少ない金額を、店員がお釣りとして支払います。

あなたと店員が使う紙幣の組合せを適切に設定するとき、両者の使う紙幣の枚数の合計は最小で何枚になるでしょう？

なお、あなたも店員も任意の紙幣を十分多く持っているとします。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
支払う紙幣の枚数とお釣りとして受け取る紙幣の枚数の合計の最小値を出力せよ。

## 题目大意
## 题目描述
给定正整数 $N$，设 $f(x)$ 表示 $x$ 在十进制下各个数位上的数的和，求一个正整数 $x$ 满足 $x\ge N$ 且最小化 $f(x)+f(x-N)$。
## 数据范围
$1\le N\le10^{1000000}$。
## 输入输出格式
### 输入格式
一行一个正整数 $N$，含义如题所述。
### 输出格式
一行一个正整数 $ans$，表示最小的 $f(x)+f(x-N)$。

```input1
36
```

```output1
8
```

```input2
91
```

```output2
3
```

```input3
314159265358979323846264338327950288419716939937551058209749445923078164062862089986280348253421170
```

```output3
243
```

## 提示
### 制約

- $ N $ は $ 1 $ 以上 $ 10^{1,000,000} $ 以下の整数

### Sample Explanation 1

あなたが価値 $ 10 $ の紙幣 $ 4 $ 枚を支払い、店員が価値 $ 1 $ の紙幣 $ 4 $ 枚をお釣りに渡すと、使う紙幣の枚数は合計で $ 8 $ 枚になります。 $ 8 $ 枚より少ない合計枚数を達成することはできないので、答えは $ 8 $ です。

### Sample Explanation 2

あなたが価値 $ 100 $ の紙幣 $ 1 $ 枚と価値 $ 1 $ の紙幣 $ 1 $ 枚を支払い、店員が価値 $ 10 $ の紙幣 $ 1 $ 枚をお釣りに渡すと、使う紙幣の枚数は合計で $ 3 $ 枚になります。

