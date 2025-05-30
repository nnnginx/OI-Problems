## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc136/tasks/abc136_d

マスの情報を表す、`L` と `R` で構成された文字列 $ S $ が与えられます。

文字列 $ S $ の長さを $ N $ としたとき、$ N $ 個のマスが左右一列に並んでおり、左から $ i $ 番目のマスには $ S $ の左から $ i $ 番目の文字が書かれています。

ただし、左端のマスには必ず `R`、右端のマスには必ず `L` が書かれています。

はじめ、各マスには $ 1 $ 人の子どもが居ます。

子どもたちはそれぞれ次の規則に従った移動を $ 10^{100} $ 回行います。

- 今居るマスに書かれた文字に従って $ 1 $ マス移動する。すなわち、今居るマスに書かれた文字が `L` のとき左隣のマスに、`R` のとき右隣のマスに移動する。

$ 10^{100} $ 回の移動の後に各マスに居る子どもの人数を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ 10^{100} $ 回の移動の後に各マスに居る子どもの人数を左のマスから順に出力せよ。

## 题目大意
给定一个长为 $n$ 的只有 $L$ 和 $R$ 的字符串 $S$ ，字符串每一个字符上都有一个点。  
现在开始 $10^{100}$ 轮移动，每一轮移动，每个字符上的点按照它当前字符上的字母来决定向左还是向右移动，如果为 $L$ 则向左移动一格， $R$ 则向右移动一格。保证字符串开头字符为 $R$ ，末尾字符为 $L$ 。  
输出经过 $10^{100}$ 轮移动后每个字符上点的个数。  
$\ $  
对于样例一，  
第一次移动后个字符上点的个数为 $0,2,1,1,1$    
第二次移动后个字符上点的个数为 $0,1,2,1,1$  
最后一次移动每个字符上点的个数 $0,1,2,1,1$

```input1
RRLRL
```

```output1
0 1 2 1 1
```

```input2
RRLLLLRLRRLL
```

```output2
0 3 3 0 0 0 1 1 0 2 2 0
```

```input3
RRRLLRLLRRRLLLLL
```

```output3
0 0 3 2 0 2 1 0 0 0 4 4 0 0 0 0
```

## 提示
### 制約

- $ S $ は長さ $ 2 $ 以上 $ 10^5 $ 以下の文字列であり、$ S $ の各文字は `L` または `R` である。
- $ S $ の $ 1 $ 文字目は `R`、$ N $ 文字目は `L` である。

### Sample Explanation 1

\- $ 1 $ 回の移動の後に各マスに居る子どもの人数は左のマスから順に $ 0,\ 2,\ 1,\ 1,\ 1 $ 人です。 - $ 2 $ 回の移動の後に各マスに居る子どもの人数は左のマスから順に $ 0,\ 1,\ 2,\ 1,\ 1 $ 人です。 - この移動を $ 10^{100} $ 回行った後に各マスに居る子どもの人数は左のマスから順に $ 0,\ 1,\ 2,\ 1,\ 1 $ 人です。

