## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc270/tasks/abc270_e

$ 1,2,\ldots,N $ の番号がついた $ N $ 個のかごが円状に置かれています。  
 $ 1\leq\ i\ \leq\ N-1 $ についてかご $ i $ の右隣にはかご $ i+1 $ があり、かご $ N $ の右隣にはかご $ 1 $ があります。

かご $ i $ の中には $ A_i $ 個りんごが入っています。

高橋君は最初かご $ 1 $ の前におり、以下の行動を繰り返します。

- 目の前にあるかごの中にりんごがあれば $ 1 $ 個かごから取り出して食べる。その後、りんごを食べたかどうかにかかわらず、右隣のかごの前に移動する。

高橋君がちょうど $ K $ 個のりんごを食べた時点で、各かごの中に残っているりんごの個数を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式
$ N $ 個の整数を空白区切りで出力せよ。  
 $ i $ 番目には、高橋君がちょうど $ K $ 個のりんごを食べた時点で、かご $ i $ の中に残っているりんごの個数を出力せよ。

## 题目大意
有 $N$ 个编号为 $1,2,\dots, N$ 的篮子排成一个环。

对于每一个 篮子 $i$ $(1 \le i \le N-1 $ ) ， 有篮子 $i+1$ 在它的右边。（篮子 $1$ 在 篮子 $N$ 的右边）。

现在第 $i$ 个篮子里有 $A_i$ 个苹果。

高桥君从第 $1$ 个篮子开始，如果他面对的篮子里有至少一个苹果，就拿一个吃掉。然后，不管他有没有吃到苹果，都要去紧靠在右边的下一个篮子，直到他吃到 $K$ 个苹果。

当高桥君吃到 $K$ 个苹果后，求每个篮子里还有多少个苹果。（数据保证所有苹果的数量总和 $\ge K$ )

------------

## 数据说明

- $ 1 \le N \le 10^5 $
- $ 1 \le A_i \le 10^{12} $
- $ 1 \le K \le 10^{12} $
- $\sum^{N}_{i=1} A_i \ge K$
- 输入的所有值均为正整数。

```input1
3 3
1 3 0
```

```output1
0 1 0
```

```input2
2 1000000000000
1000000000000 1000000000000
```

```output2
500000000000 500000000000
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 0\ \leq\ A_i\ \leq\ 10^{12} $
- $ 1\ \leq\ K\ \leq\ 10^{12} $
- りんごは全部で $ K $ 個以上ある。すなわち、$ \sum_{i=1}^{N}A_i\geq\ K $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

高橋君は次のように行動します。 - 目の前にあるかご $ 1 $ の中にりんごがあるので $ 1 $ 個かごから取り出して食べる。その後、かご $ 2 $ の前に移動する。この時点で各かごの中のりんごの個数は $ (0,3,0) $ である。 - 目の前にあるかご $ 2 $ の中にりんごがあるので $ 1 $ 個かごから取り出して食べる。その後、かご $ 3 $ の前に移動する。この時点で各かごの中のりんごの個数は $ (0,2,0) $ である。 - 目の前にあるかご $ 3 $ の中にりんごはない。かご $ 1 $ の前に移動する。この時点で各かごの中のりんごの個数は $ (0,2,0) $ である。 - 目の前にあるかご $ 1 $ の中にりんごはない。かご $ 2 $ の前に移動する。この時点で各かごの中のりんごの個数は $ (0,2,0) $ である。 - 目の前にあるかご $ 2 $ の中にりんごがあるので $ 1 $ 個かごから取り出して食べる。その後、かご $ 3 $ の前に移動する。この時点で各かごの中のりんごの個数は $ (0,1,0) $ である。

