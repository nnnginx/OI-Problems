# AT_abc319_d [ABC319D] Minimum Width

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc319/tasks/abc319_d

高橋くんは、$ N $ 個の単語からなる文章をウィンドウに表示させようとしています。 すべての単語の縦幅は等しく、$ i $ 番目 $ (1\leq\ i\leq\ N) $ の単語の横幅は $ L\ _\ i $ です。

文章は、横幅 $ 1 $ の空白を単語の区切りとしてウィンドウに表示されます。 より厳密には、高橋くんが横幅 $ W $ のウィンドウに文章を表示しているとき、次の条件が成り立っています。

- 文章はいくつかの行に分かれている。
- $ 1 $ 番目の単語は一番上の行の先頭に表示されている。
- $ i $ 番目 $ (2\leq\ i\leq\ N) $ の単語は、$ i-1 $ 番目の単語の次に間隔を $ 1 $ だけ開けて表示されているか、$ i-1 $ 番目の単語が含まれる行の下の行の先頭に表示されているかの一方である。それ以外の場所に表示されていることはない。
- それぞれの行の横幅は $ W $ を超えない。ここで、行の横幅とは最も左にある単語の左端から最も右にある単語の右端までの距離を指す。
 
高橋くんが文章をウィンドウに表示したとき、文章が $ M $ 行に収まりました。 ウィンドウの横幅としてありえる最小の値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ L\ _\ 1 $ $ L\ _\ 2 $ $ \ldots $ $ L\ _\ N $

## 输出格式

答えを $ 1 $ 行で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
13 3
9 5 2 7 1 8 8 2 1 5 2 3 6
```

### 输出 #1

```
26
```

## 输入输出样例 #2

### 输入 #2

```
10 1
1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000
```

### 输出 #2

```
10000000009
```

## 输入输出样例 #3

### 输入 #3

```
30 8
8 55 26 97 48 37 47 35 55 5 17 62 2 60 23 99 73 34 75 7 46 82 84 29 41 32 31 52 32 60
```

### 输出 #3

```
189
```

## 说明/提示

### 制約

- $ 1\leq\ M\leq\ N\leq2\times10\ ^\ 5 $
- $ 1\leq\ L\ _\ i\leq10^9\ (1\leq\ i\leq\ N) $
- 入力はすべて整数
 
### Sample Explanation 1

ウィンドウの横幅が $ 26 $ のとき、以下のようにして与えられた文章を $ 3 $ 行に収めることができます。 !\[\](https://img.atcoder.jp/abc319/710c42acf58eacf40178e28a0a0b3a2c.png) ウィンドウの横幅が $ 25 $ 以下のときは与えられた文章を $ 3 $ 行に収めることができないため、$ 26 $ を出力してください。 単語を複数の行にまたがって表示させたり、行の横幅がウィンドウの横幅を上回ったり、単語を並べ替えたりしてはいけないことに注意してください。 !\[\](https://img.atcoder.jp/abc319/ed3aac3d0c0eb00c5663aa6a95023b33.png)

### Sample Explanation 2

答えが $ 32\operatorname{bit} $ 整数に収まらない場合があることに注意してください。