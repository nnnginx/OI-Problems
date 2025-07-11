# AT_abc324_g [ABC324G] Generate Arrays

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc324/tasks/abc324_g

高橋くんは、長さ $ N $ の数列 $ A=(A\ _\ 1,A\ _\ 2,\ldots,A\ _\ N) $ を持っています。 $ A $ は $ (1,2,\ldots,N) $ の順列です。

高橋くんは、操作を $ Q $ 回行って、$ 1+Q $ 個の数列を作ろうとしています。 **$ 0 $ 番の数列を $ A $ として**、高橋くんは一連の操作を始めます。 $ i $ 回目 $ (1\leq\ i\leq\ Q) $ の操作は、整数の $ 3 $ つ組 $ (t\ _\ i,s\ _\ i,x\ _\ i) $ を用いて表され、次のような操作に対応します（ 入出力例の説明も参考にしてください）。

- $ t\ _\ i=1 $ のとき、高橋くんは $ s\ _\ i $ 番 $ (0\leq\ s\ _\ i\lt\ i) $ の数列から $ x\ _\ i $ 個目より後の要素を取り除き、取り除いた要素を順序を保って新しく $ i $ 番の数列とする。
- $ t\ _\ i=2 $ のとき、高橋くんは $ s\ _\ i $ 番 $ (0\leq\ s\ _\ i\lt\ i) $ の数列から値が $ x\ _\ i $ より大きい要素を取り除き、取り除いた要素を順序を保って新しく $ i $ 番の数列とする。

ただし、長さ $ L $ の数列 $ X $ について、$ X $ のどの要素も「$ 0 $ 個目より後の要素」です。 また、$ L\leq\ l $ を満たす任意の $ l $ について $ X $ のどの要素も「$ l $ 個目より後の要素」ではありません。

$ i=1,2,\ldots,Q $ について、$ i $ 回目の操作が終わった**直後**の $ i $ 番の数列の長さを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A\ _\ 1 $ $ A\ _\ 2 $ $ \ldots $ $ A\ _\ N $ $ Q $ $ t\ _\ 1 $ $ s\ _\ 1 $ $ x\ _\ 1 $ $ t\ _\ 2 $ $ s\ _\ 2 $ $ x\ _\ 2 $ $ \vdots $ $ t\ _\ Q $ $ s\ _\ Q $ $ x\ _\ Q $

## 输出格式

答えを $ Q $ 行で出力せよ。 $ i $ 行目 $ (1\leq\ i\leq\ Q) $ には、$ i $ 回目の操作が終わった直後における $ i $ 番の列の長さを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10
1 8 7 4 5 6 3 2 9 10
5
2 0 4
1 1 2
2 0 2
2 2 5
1 0 1
```

### 输出 #1

```
6
4
2
3
1
```

## 输入输出样例 #2

### 输入 #2

```
8
6 7 8 4 5 1 3 2
5
2 0 0
1 1 0
2 2 0
1 3 8
2 2 3
```

### 输出 #2

```
8
8
8
0
0
```

## 输入输出样例 #3

### 输入 #3

```
30
20 6 13 11 29 30 9 10 16 5 8 25 1 19 12 18 7 2 4 27 3 22 23 24 28 21 14 26 15 17
10
1 0 22
1 0 21
2 0 15
1 0 9
1 3 6
2 3 18
1 6 2
1 0 1
2 5 20
2 7 26
```

### 输出 #3

```
8
1
8
4
2
5
3
8
1
1
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq2\times10^5 $
- $ 1\leq\ A\ _\ i\leq\ N\ (1\leq\ i\leq\ N) $
- $ A\ _\ i\neq\ A\ _\ j\ (1\leq\ i\lt\ j\leq\ N) $
- $ 1\leq\ Q\leq2\times10^5 $
- $ t\ _\ i=1,2\ (1\leq\ i\leq\ Q) $
- $ 0\leq\ s\ _\ i\lt\ i\ (1\leq\ i\leq\ Q) $
- $ 0\leq\ x\ _\ i\leq\ N\ (1\leq\ i\leq\ Q) $
- 入力はすべて整数

### Sample Explanation 1

はじめ、高橋くんは長さ $ 10 $ の数列 $ A=(1,8,7,4,5,6,3,2,9,10) $ を持っています。 高橋くんは、$ 0 $ 番の数列を $ A=(1,8,7,4,5,6,3,2,9,10) $ として一連の操作を開始します。 $ 1 $ 回目の操作では、$ 0 $ 番の数列の $ 4 $ より大きな要素 $ 8,7,5,6,9,10 $ を取り除き、これらを新しく $ 1 $ 番の数列にします。この操作が終わったとき、$ 0,1 $ 番の数列はそれぞれ $ (1,4,3,2),(8,7,5,6,9,10) $ になります。 $ 2 $ 回目の操作では、$ 1 $ 番の数列の $ 2 $ 個目より後の要素 $ 5,6,9,10 $ を取り除き、これらを新しく $ 2 $ 番の数列にします。この操作が終わったとき、$ 0,1,2 $ 番の数列はそれぞれ $ (1,4,3,2),(8,7),(5,6,9,10) $ になります。 $ 3 $ 回目以降の操作について、$ i $ 回目の操作が終わったときの $ 0,1,2,\ldots,i $ 番の数列はそれぞれ以下のようになります。 - $ (1,2),(8,7),(5,6,9,10),(4,3) $ - $ (1,2),(8,7),(5),(4,3),(6,9,10) $ - $ (1),(8,7),(5),(4,3),(6,9,10),(2) $ $ i=1,2,\ldots,5 $ 回目の操作が終わったときの $ i $ 番の数列の長さはそれぞれ $ 6,4,2,3,1 $ なので、これらをそれぞれの行に出力してください。

### Sample Explanation 2

操作の結果、空の数列が生じることもあります。