# AT_arc160_e [ARC160E] Make Biconnected

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc160/tasks/arc160_e

$ N $ 頂点の無向木 $ G $ が与えられます。**$ G $ の全ての頂点の次数は $ 3 $ 以下です。**   
 頂点には $ 1 $ から $ N $ の番号がついています。辺には $ 1 $ から $ N-1 $ までの番号がついていて、辺 $ i $ は頂点 $ u_i $ と頂点 $ v_i $ を結んでいます。  
 また、全ての頂点には重みが設定されていて、頂点 $ i $ の重みは $ W_i $ です。

あなたは $ G $ に $ 0 $ 本以上の辺を追加します。頂点 $ i $ と頂点 $ j $ の間に辺を追加すると $ W_i\ +\ W_j $ のコストがかかります。

次の条件を満たすように辺を追加する方法のうち、コストの総和が最小である方法を $ 1 $ つ出力してください。

- $ G $ は二重頂点連結である。つまり、$ G $ 内の任意の頂点 $ v $ について、$ G $ から頂点 $ v $ および $ v $ に隣接する辺を取り除いても $ G $ は連結な状態を保っている。
 
$ T $ 個のテストケースが与えられるので、それぞれについて答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。ここで、$ \mathrm{case}_i $ は $ i $ 番目のテストケースを意味する。

> $ T $ $ \mathrm{case}_1 $ $ \mathrm{case}_2 $ $ \vdots $ $ \mathrm{case}_N $

各テストケースは以下の形式で与えられる。

> $ N $ $ W_1 $ $ W_2 $ $ \dots $ $ W_N $ $ u_1 $ $ v_1 $ $ u_2 $ $ v_2 $ $ \vdots $ $ u_{N-1} $ $ v_{N-1} $

## 输出格式

各テストケースについて、以下の形式で答えを出力せよ。ここで、

- 追加する辺の本数は $ M $ 本で、
- $ i $ 本目の追加する辺は頂点 $ a_i $ と頂点 $ b_i $ を結んでいる
 
とする。

答えが複数ある場合は、どれを出力しても正答とみなされる。

> $ M $ $ a_1 $ $ b_1 $ $ a_2 $ $ b_2 $ $ \vdots $ $ a_M $ $ b_M $

## 输入输出样例 #1

### 输入 #1

```
2
3
2 3 5
1 2
2 3
7
1 10 100 1000 10000 100000 1000000
1 2
2 3
2 4
3 5
3 6
4 7
```

### 输出 #1

```
1
1 3
2
7 6
1 5
```

## 说明/提示

### 制約

- $ 1\ \leq\ T\ \leq\ 2\ \times\ 10^5 $
- $ 3\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ u_i,\ v_i\ \leq\ N $
- 入力で与えられるグラフは木
- 入力で与えられるグラフにおいて、全ての頂点は次数が $ 3 $ 以下
- $ 1\ \leq\ W_i\ \leq\ 10^9 $
- $ W_i $ は整数
- 全てのテストケースにおける $ N $ の総和は $ 2\ \times\ 10^5 $ 以下
 
### Sample Explanation 1

$ 1 $ 番目のテストケースでは、頂点 $ 1 $ と頂点 $ 3 $ を結ぶ辺を張ると $ G $ が問題文の条件を満たします。 この時、コストは $ W_1\ +\ W_3\ =\ 2\ +\ 5\ =\ 7 $ になります。 コストが $ 7 $ 未満で条件を満たす辺の張り方は存在しないため、これが答えになります。 $ 2 $ 番目のテストケースでは、コストの総和は $ (W_7\ +\ W_6)\ +\ (W_1\ +\ W_5)\ =\ 1100000\ +\ 10001\ =\ 1110001 $ になり、これが最小です。