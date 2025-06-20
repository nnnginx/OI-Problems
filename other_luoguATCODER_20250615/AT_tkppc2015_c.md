# AT_tkppc2015_c お姉ちゃんって呼んで (Call me sister)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tkppc/tasks/tkppc2015_c

joisinoお姉ちゃんは少し疲れたので、近くにあった喫茶店で休むことにした。  
 ここで、joisinoお姉ちゃんは、あるウェイトレスがとても気に入ったので、彼女に「お姉ちゃん」と呼んでもらいたいと思った。  
 しかし、彼女に「お姉ちゃん」と呼んでもらえるかどうかは、彼女の機嫌にかかわっている。

これからこの喫茶店では、$ N $個の出来事が起こる。  
 それぞれの出来事には$ 1～N $までの番号が割り振られていて、出来事$ i(1≦i≦N) $は、時刻$ T_i $に起こり、ウェイトレスの機嫌に$ K_i $が足される。  
 なお、同じ時刻に二つ以上の出来事が起こることはない  
 そして、ウェイトレスの機嫌が$ M $以上の時だけ、お姉ちゃんと呼んでもらうことができる。  
 現在の時刻は$ 0 $であり、現在のウェイトレスの機嫌は$ 0 $である。

joisinoお姉ちゃんは、時刻$ S $にこの喫茶店を出る。  
 joisinoお姉ちゃんは、店を出るまでの間に「お姉ちゃん」と呼んでもらえる時間がどれだけあるのか知りたいと思い、それを求めるプログラムを作成することにした。  
 なお、joisinoお姉ちゃんがどのようにして、これから起こる出来事の情報を手に入れたのかは謎である。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ S $ $ T_1 $ $ K_1 $ $ T_2 $ $ K_2 $ : $ T_N $ $ K_N $

- $ 1 $行目には、これから起こる出来事の数$ N(1≦N≦1000) $と、お姉ちゃんと呼んでもらえる機嫌の最低値$ M(0≦M≦10000) $が空白区切り書かれている。
- $ 2 $行目には、joisinoお姉ちゃんが喫茶店を出る時刻$ S(2≦S≦10000) $が書かれている。
- $ 3 $行目から続く$ N $行のうち$ i $行目では、これから起こる出来事の情報として、整数$ T_i(0＜T_i＜S) $と、整数$ K_i(-10000≦K_i＜0,0＜K_i≦10000) $が空白区切りで書かれている。
- $ i≠j $において、$ T_i≠T_j $が保障されている。

## 输出格式

お姉ちゃんと呼んでもらえる時間の合計を$ 1 $行で出力せよ。  
 また、出力の末尾には改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
5 20
20
5 16
8 -4
3 9
18 2
12 -3
```

### 输出 #1

```
9
```

## 说明/提示

### 配点

この問題に部分点はない。正解すると$ 60 $点が得られる。

### Sample Explanation 1

\- 時刻$ 5 $から時刻$ 12 $までの$ 7 $と、時刻$ 18 $から、喫茶店を出る時刻$ 20 $までの$ 2 $の間で、機嫌が$ 20 $以上となっているため、その合計である$ 9 $を出力する。