## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc252/tasks/abc252_e

AtCoder 王国には都市 $ 1,2,\ldots,N $ の $ N $ 個の都市と、道路 $ 1,2,\ldots,M $ の $ M $ 本の道路があります。  
道路 $ i $ は都市 $ A_i $ と $ B_i $ を双方向に結び、距離は $ C_i $ です。  
どの都市間もいくつかの道路を通って行き来することができます。

財政難である王国は、どの都市間もいくつかの道路を通って行き来できるという条件を満たすように $ N-1 $ 本の道路を保守し、それ以外の道路を廃道にすることにしました。

保守する道路のみを通って都市 $ 1 $ から都市 $ i $ へ移動するときの距離を $ d_i $ とするとき、保守する道路の選び方であって、$ d_2+d_3+\ldots+d_N $ を最小化するようなものを $ 1 $ つ出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ B_1 $ $ C_1 $ $ A_2 $ $ B_2 $ $ C_2 $ $ \vdots $ $ A_M $ $ B_M $ $ C_M $

## 输出格式
保守するような道路の番号を空白区切りで出力せよ。出力の順序は問わない。  
答えが複数存在する場合、どれを出力しても正解とみなされる。

## 题目大意
给定 $ n $ 个点 $ m $ 条边的无向连通简单图，每条边为 $ a_i $ 到 $ b_i $，权值为 $ c_i $。你需要构造一棵生成树，最小化点 $ 1 $ 在生成树上到其它所有点的距离和，输出生成树的所有边的序号。如果有多个方案随便输出一个即可。

```input1
3 3
1 2 1
2 3 2
1 3 10
```

```output1
1 2
```

```input2
4 6
1 2 1
1 3 1
1 4 1
2 3 1
2 4 1
3 4 1
```

```output2
3 1 2
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ N-1\ \leq\ M\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ A_i\ <\ B_i\ \leq\ N $
- $ i\neq\ j $ のとき、$ (A_i,B_i)\neq(A_j,B_j) $
- $ 1\leq\ C_i\ \leq\ 10^9 $
- どの都市間もいくつかの道路を通って行き来することができる
- 入力に含まれる値は全て整数である

### Sample Explanation 1

保守する道路の選び方と $ d_i $ の値は次のようになります。 - 道路 $ 1,2 $ を保守するとき、$ d_2=1 $, $ d_3=3 $ - 道路 $ 1,3 $ を保守するとき、$ d_2=1 $, $ d_3=10 $ - 道路 $ 2,3 $ を保守するとき、$ d_2=12 $, $ d_3=10 $ よって、道路 $ 1,2 $ を保守するときに $ d_2+d_3 $ が最小になります。

