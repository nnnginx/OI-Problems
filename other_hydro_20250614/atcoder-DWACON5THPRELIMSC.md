## 题目描述
[problemUrl]: https://atcoder.jp/contests/dwacon5th-prelims/tasks/dwacon5th_prelims_c

ドワンゴのコンテンツ配信基盤システム Dwango Media Cluster は、略して DMC と呼ばれています。  
 この名前をかっこ良いと感じたニワンゴくんは、文字列の DMC らしさを数値として定義することにしました。  
 具体的には、長さ $ N $ のある文字列 $ S $ と3以上の整数 $ k $ が与えられた時、以下を満たす整数の3つ組 $ (a,b,c) $ の個数を $ S $ の $ k $-DMC 数と呼ぶことにします。

- $ 0\ \leq\ a $
- $ S[a] $ = `D`
- $ S[b] $ = `M`
- $ S[c] $ = `C`
- $ c-a $

ここで、$ S[a] $ は $ S $ の $ a $ 番目の文字を表します。先頭の文字は $ 0 $ 文字目として扱います (つまり、$ 0\ \leq\ a\ \leq\ N\ -\ 1 $ です)。

ある文字列 $ S $ と $ Q $ 個の整数 $ k_0,\ k_1,\ ...,\ k_{Q-1} $ に対して、$ k_i $-DMC 数をそれぞれ計算してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $ $ Q $ $ k_{0} $ $ k_{1} $ $ ... $ $ k_{Q-1} $

## 输出格式
$ Q $ 行出力せよ。  
 $ i $ 行目 $ (0\ \leq\ i\ \leq\ Q-1) $ には、文字列 $ S $ の $ k_i $-DMC 数を出力せよ。

## 题目大意
给定一个字符串长度 $N$ 和字符串 $S$ 以及 $Q$ 次查询，每次给定一个 $k$ 值。对于每次查询，输出满足所有以下条件的 $(D,M,C)$ 组数。

$0≤a<b<c≤N-1$ 
$S[a]=D，S[b]=M，S[c]=C$   
$c-a<k$

```input1
18
DWANGOMEDIACLUSTER
1
18
```

```output1
1
```

```input2
18
DDDDDDMMMMMCCCCCCC
1
18
```

```output2
210
```

```input3
54
DIALUPWIDEAREANETWORKGAMINGOPERATIONCORPORATIONLIMITED
3
20 30 40
```

```output3
0
1
2
```

```input4
30
DMCDMCDMCDMCDMCDMCDMCDMCDMCDMC
4
5 10 15 20
```

```output4
10
52
110
140
```

## 提示
### 制約

- $ 3\ \leq\ N\ \leq\ 10^6 $
- $ S $ は`A` - `Z` からなる文字列
- $ 1\ \leq\ Q\ \leq\ 75 $
- $ 3\ \leq\ k_i\ \leq\ N $
- 入力として与えられる数値はすべて整数である

### Sample Explanation 1

$ (a,b,c)\ =\ (0,\ 6,\ 11) $ が条件を満たします。 Dwango Media Cluster は、ニワンゴくんの定義では意外と DMC らしくないようです。

### Sample Explanation 2

$ 6\times\ 5\times\ 7 $ 個の組み合わせがありえます。

### Sample Explanation 3

$ c-a\ 以外の条件は\ (a,\ b,\ c)\ =\ (0,\ 23,\ 36),\ (8,\ 23,\ 36) $ が満たします。 ちなみに、DWANGO は「Dial-up Wide Area Network Gaming Operation」の頭文字です。

