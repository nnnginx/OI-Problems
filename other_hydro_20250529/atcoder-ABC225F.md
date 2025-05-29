## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc225/tasks/abc225_f

カードが $ N $ 枚あり、$ i $ 番目のカードには文字列 $ S_i $ が書かれています。

この中からちょうど $ K $ 枚選び、好きな順序で繋げてできる文字列のうち辞書順最小のものを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式
答えを出力せよ。

## 题目大意
给出 $N$ 个串，请你在其中选出 $K$ 个串，使得这 $K$ 个串前后拼接形成的串字典序最小。

```input1
4 3
ode
zaaa
r
atc
```

```output1
atcoder
```

```input2
5 2
z
z
zzz
z
zzzzzz
```

```output2
zz
```

## 提示
### 制約

- $ 1\ \leq\ K\ \leq\ N\ \leq\ 50 $
- $ 1\ \leq\ |S_i|\ \leq\ 50 $
- $ S_i $ は英小文字からなる

### Sample Explanation 1

カードの中に書かれている文字を、反転させたり並び替えたりすることはできません。 たとえば $ 1 $ 枚目のカードに書かれている `ode` を、`edo` や `deo` のように使うことはできません。

### Sample Explanation 2

$ S_i\ =\ S_j $ を満たす $ i,j(i\neq\ j) $ の組が存在することもあります。

