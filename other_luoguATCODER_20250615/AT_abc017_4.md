# AT_abc017_4 [ABC017D] サプリメント

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc017/tasks/abc017_4

健康志向の高橋君は通販で購入したサプリメントを摂取することにした。

サプリメントは $ N $ 個あり、$ 1 $ から $ N $ まで番号が付けられている。

また、サプリメントの味は $ M $ 種類あり、$ 1 $ から $ M $ まで番号が付けられている。サプリメント $ i\ (1\ ≦\ i\ ≦\ N) $ の味は $ f_i\ (1\ ≦\ f_i\ ≦\ M) $ である。

高橋君はサプリメントを番号順に複数日かけて摂取する予定である。高橋君はサボらないように、サプリメントが $ 1 $ つ以上残っている場合はその日中に必ず $ 1 $ つ以上サプリメントを摂取しなければならないという規則を定めた。

高橋君は強靭な肉体を持っているため、$ 1 $ 日にどれだけサプリメントを摂取しても大丈夫だが、同じ味には飽きてしまうので、同じ日に同じ味のサプリメントを $ 2 $ つ以上摂取することはできない。

高橋君は、サプリメントの摂取方法の是非について吟味するため、このような条件下で全部で何通りの摂取方法があるかを知りたい。

ここで $ 2 $ つの摂取方法についてそれらが違うというのは、ある日について摂取したサプリメントの番号の組み合わせが異なることを定義する。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ f_1 $ $ f_2 $ : $ f_N $

- $ 1 $ 行目には、$ 2 $ つの整数 $ N\ (1\ ≦\ N\ ≦\ 100,000) $ と $ M\ (1\ ≦\ M\ ≦\ 100,000) $ が空白区切りで書かれている。これはサプリメントが $ N $ 個あり、味の種類が $ M $ 種類あることを表す。
- $ 2 $ 行目から $ N $ 行には、サプリメントの味に関する情報が与えられる。これら $ N $ 行のうち上から $ i\ (1\ ≦\ i\ ≦\ N) $ 行目には整数 $ f_i\ (1\ ≦\ f_i\ ≦\ M) $ が書かれている。これは、サプリメント $ i $ の味が $ f_i $ であることを表す。

## 输出格式

摂取方法の総数を $ 1,000,000,007\ (=\ 1000000007) $ で割ったあまりを $ 1 $ 行に出力せよ。出力の末尾にも改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
5 2
1
2
1
2
2
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
6 6
1
2
3
4
5
6
```

### 输出 #2

```
32
```

## 说明/提示

### 部分点

この問題には部分点が設定されている。

- $ N\ ≦\ 5,000 $ かつ $ M\ ≦\ 5,000 $ を満たすデータセット $ 1 $ に正解した場合は、上記とは別に $ 30 $ 点が与えられる。
- 追加制約のないデータセット $ 2 $ に正解した場合は、上記とは別に $ 70 $ 点が与えられる。

### Sample Explanation 1

以下の $ 5 $ 通りが考えられます。 $ 1 $ 日目 $ 2 $ 日目 $ 3 $ 日目 $ 4 $ 日目 $ 5 $ 日目 サプリメント $ 1 $ サプリメント $ 2 $ サプリメント $ 3 $ サプリメント $ 4 $ サプリメント $ 5 $ サプリメント $ 1 $ サプリメント $ 2 $ サプリメント $ 3,4 $ サプリメント $ 5 $ なし サプリメント $ 1 $ サプリメント $ 2,3 $ サプリメント $ 4 $ サプリメント $ 5 $ なし サプリメント $ 1,2 $ サプリメント $ 3 $ サプリメント $ 4 $ サプリメント $ 5 $ なし サプリメント $ 1,2 $ サプリメント $ 3,4 $ サプリメント $ 5 $ なし なし

### Sample Explanation 2

どのように食べても飽きません。