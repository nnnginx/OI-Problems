# AT_tenka1_2013_qualB_b 天下一後入れ先出しデータ構造

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tenka1-2013-qualb/tasks/tenka1_2013_qualB_b

 スタックは最も基本的なデータ構造の1つであり、データを後入れ先出し (Last In First Out) の構造で保持するものである。スタックは最初は空で、要素の追加と取り出しができるが、取り出しは追加されたのが遅い順に行われる。

 ある日、天下一株式会社に務めるユウヤ君は、スタックになりきるという仕事を言い渡された。唖然とするユウヤ君を心配するあなたは、以下の形式の入力で与えられる命令の列をユウヤ君の代わりに処理して、後述のような出力を行うプログラムを作成することにした。

- - - - - -

 入力は以下の形式で標準入力から与えられる。

> $ Q $ $ L $ $ query_1 $ $ query_2 $ $ ... $ $ query_Q $

- $ 1 $ 行目は、与えられる命令の数 $ Q $ ($ 1\ \leq\ Q\ \leq\ 10^5 $) と スタックのサイズ $ L $ ($ 1\ \leq\ L\ \leq\ 2147483647 $) が空白区切りで与えられる。
- $ 2 $ 行目から $ Q+1 $ 行目までの $ Q $ 行は、$ i $ ($ 1\ \leq\ i\ \leq\ Q $) 番目の 命令が与えられる。

 各命令は、以下 $ 4 $ 種類のうちいずれかに該当する。

1. Push $ N $ $ M $

- スタックに要素 $ M $ を $ N $ 個追加する。出力は行わない。

10. Pop $ N $
- スタックから要素を $ N $ 個取り出す。出力は行わない。

12. Top
- スタックの先頭要素を $ 1 $ 行で出力する。この命令でスタックを構成する要素は変更されない。

14. Size
- スタックの要素数を $ 1 $ 行で出力する。

$ N $, $ M $ はそれぞれ整数で、 $ 1\ \leq\ N\ \leq\ 10^5 $, $ -2^{20}\ \leq\ M\ \leq\ 2^{20} $ をみたす。

ただし、スタックの先頭要素とは、スタックの要素のうちで最後に追加されたものであり、もしそのときPop $ 1 $を行ったとすると取り出される要素である。

- $ Q\ \leq\ 50 $, $ N\ \leq\ 50 $ の入力に正解すると、$ 60 $ 点満点に対して部分点として、$ 30 $ 点が与えられる。

 上記のとおり、与えられた命令を順番に処理していき、Top、またはSizeの入力が与えられた際に出力を行う。

 ただし、以下の $ 3 $ つの場合、スタックは例外を投げて止まってしまう。

- Push $ N $ $ M $ を要素数が $ L-N $ より大きいスタックに対して行った場合
- Pop $ N $を要素数が $ N $ 未満のスタックに対して行った場合
- Top を空のスタックに対して行った場合

 スタックが投げる例外は以下の通りである。

- Push による例外でプログラムが終了した場合は `FULL`
- Pop または Top による例外でプログラムが終了した場合は `EMPTY`

 これらの例外は $ 1 $ 行で出力され、例外を投げた後のスタックはそれ以降の命令を放棄する。  
 スタックは最後まで正常に命令を処理できた場合、 `SAFE` を $ 1 $ 行で出力して終了する。

 ```

7 20
Push 2 3
Push 4 5
Top
Size
Pop 5
Top
Size
```

 ```

5
6
3
1
SAFE
```

 ```

1 10
Push 40 40
```

 ```

FULL
```

 ```

5 10
Push 1 2
Top
Pop 1
Top
Size
```

 ```

2
EMPTY
```

 ```

4 10
Top
Size
Push 1 1
Top
```

 ```

EMPTY
```

## 输入格式

无

## 输出格式

无