# AT_abc291_h [ABC291Ex] Balanced Tree

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc291/tasks/abc291_h

$ N $ 頂点の木 $ T $ が与えられます。$ i $ 番目の辺は頂点 $ A_i $ と $ B_i $ を結んでいます。

次の条件をともに満たす $ N $ 頂点の根付き木 $ R $ を $ 1 $ つ求めてください。

- $ 1\ \leq\ x\ <\ y\ \leq\ N $ を満たす全ての整数の組 $ (x,y) $ に対し次が成り立つ
  - $ R $ における頂点 $ x,y $ の最小共通祖先が頂点 $ z $ であるとき、$ T $ において 頂点 $ x,y $ を結ぶ単純パス上に頂点 $ z $ が存在する
- $ R $ において、根以外の全ての頂点 $ v $ に対し、$ v $ を根とする部分木の頂点数の $ 2 $ 倍は、 $ v $ の親を根とする部分木の頂点数以下である
 
なお、この条件を満たす根付き木は必ず存在することが証明できます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ \vdots $ $ A_{N-1} $ $ B_{N-1} $

## 输出格式

問題文中の条件を満たす根付き木を $ R $ とする。$ R $ における頂点 $ i $ の親を頂点 $ p_i $ とする（ただし、$ i $ が根のときは $ p_i=-1 $ と定める）。  
 $ N $ 個の整数 $ p_1,\ldots,p_N $ をこの順に空白区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
1 2
2 3
3 4
```

### 输出 #1

```
2 -1 4 2
```

## 输入输出样例 #2

### 输入 #2

```
5
1 2
1 3
1 4
1 5
```

### 输出 #2

```
-1 1 1 1 1
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\leq\ A_i,B_i\ \leq\ N $
- 入力は全て整数である
- 与えられるグラフは木である
 
### Sample Explanation 1

例えば、$ R $ における頂点 $ 1,3 $ の最小共通祖先は頂点 $ 2 $ であり、$ T $ において、頂点 $ 1,3 $ を結ぶ単純パス上に頂点 $ 2 $ が存在します。 また、例えば、$ R $ における頂点 $ 4 $ を根とする部分木の頂点数は $ 2 $ であり、その $ 2 $ 倍は、頂点 $ 2 $ を根とする部分木の頂点数 $ 4 $ 以下です。 !\[図\](https://img.atcoder.jp/abc291/7c68a1da41dbfff60a08aad4fe182376.png)