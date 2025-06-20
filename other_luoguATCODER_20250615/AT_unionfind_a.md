# AT_unionfind_a Union Find

## 题目描述

[problemUrl]: https://atcoder.jp/contests/atc001/tasks/unionfind_a

この問題は、講座用問題です。ページ下部に解説が掲載されています。

$ N $ 頂点の、単純とは限らない無向グラフを考えます。 初期状態では、頂点のみが存在し、辺は全く存在せず、全ての頂点が孤立しているとします。 以下の $ 2 $ 種類のクエリが、$ Q $ 回与えられます。

- 連結クエリ： 頂点 $ A $ と、頂点 $ B $ を繋ぐ辺を追加します。
- 判定クエリ： 頂点 $ A $ と、頂点 $ B $ が、連結であるかどうか判定します。連結であれば `Yes`、そうでなければ `No` を出力します。

クエリを順番に処理し、判定クエリへの回答を出力して下さい。 この際、同じ辺が何度も追加されることや、自分自身への辺が追加されることもある事に注意してください。

連結であるとは、頂点 $ A $ から頂点 $ B $ まで辺をたどって到達可能であることを意味します。 $ A $ と $ B $ が同じ頂点の場合、連結であると定義します。 グラフは無向であるため、連結クエリによって頂点 $ A,\ B $ 間の辺が追加されると、$ A $ から $ B $ へも $ B $ から $ A $ へも辿れるようになります。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ Q $ $ P_1 $ $ A_1 $ $ B_1 $ $ P_2 $ $ A_2 $ $ B_2 $ : $ P_Q $ $ A_Q $ $ B_Q $

- $ 1 $ 行目には、頂点の個数を表す整数 $ N\ (1≦N≦100,000) $ と、クエリの個数を表す整数 $ Q\ (1\ ≦\ Q\ ≦\ 200,000) $ が、スペース区切りで与えられる。
- $ 2 $ 行目からの $ Q $ 行のうち $ i $ 行目には、$ i $ 番目のクエリの種類を表す整数 $ P_i\ (0\ ≦\ P_i\ ≦\ 1) $ と、クエリの対象となる頂点の番号を表す整数 $ A_i,\ B_i\ (0\ ≦\ A_i,\ B_i\ ≦\ N\ -\ 1) $ が、 スペース区切りで与えられる。 
  - $ P_i\ =\ 0 $ の時、そのクエリが連結クエリであることを表す。
  - $ P_i\ =\ 1 $ の時、そのクエリが判定クエリであることを表す。

## 输出格式

各判定クエリに対し、出力をおこなって下さい。 毎回の出力の後に改行を行うこと。

## 输入输出样例 #1

### 输入 #1

```
8 9
0 1 2
0 3 2
1 1 3
1 1 4
0 2 4
1 4 1
0 4 2
0 0 0
1 0 0
```

### 输出 #1

```
Yes
No
Yes
Yes
```

## 说明/提示

### 解説

  **[Union find(素集合データ構造)](https://www.slideshare.net/secret/CIWAduFPvzGrrE "Union find(素集合データ構造)")**  from **[AtCoder Inc.](http://www.slideshare.net/chokudai)** 

### Sample Explanation 1

以下のような手順で実行されます。 - $ 1 $ つ目のクエリで、頂点 $ 1 $ と頂点 $ 2 $ を繋ぎます。 - $ 2 $ つ目のクエリで、頂点 $ 3 $ と頂点 $ 2 $ を繋ぎます。 - $ 3 $ つ目のクエリで、頂点 $ 1 $ と頂点 $ 3 $ の連結判定を行います。連結しているので、`Yes`と出力します。 - $ 4 $ つ目のクエリで、頂点 $ 1 $ と頂点 $ 4 $ の連結判定を行います。連結していないので、`No`と出力します。 - $ 5 $ つ目のクエリで、頂点 $ 2 $ と頂点 $ 4 $ を繋ぎます。 - $ 6 $ つ目のクエリで、頂点 $ 4 $ と頂点 $ 1 $ の連結判定を行います。連結しているで、`Yes`と出力します。 - $ 7 $ つ目のクエリで、頂点 $ 4 $ と頂点 $ 2 $ を繋ぎます。これらは既に繋がれていますが、多重辺が出来ることもあります。 - $ 8 $ つ目のクエリで、頂点 $ 0 $ と頂点 $ 0 $ を繋ぎます。これらは同じ頂点ですが、自己ループが出来ることもあります。 - $ 9 $ つ目のクエリで、頂点 $ 0 $ と頂点 $ 0 $ の連結判定を行います。同じ頂点は常に連結していると見做せるので、`Yes`と出力します。