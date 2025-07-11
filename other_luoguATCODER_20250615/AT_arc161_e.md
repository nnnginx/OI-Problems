# AT_arc161_e [ARC161E] Not Dyed by Majority (Cubic Graph)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc161/tasks/arc161_e

$ N $ を正の**偶数**として，$ N $ 頂点 $ \displaystyle\frac{3}{2}N $ 辺の連結な単純無向グラフが与えられます． 頂点には $ 1 $ から $ N $ までの番号が付いており，$ i $ 番目の辺は頂点 $ A_i $ と頂点 $ B_i $ を結んでいます． また，すべての頂点について，**接続する辺の本数はちょうど $ 3 $** です．

与えられたグラフの各頂点を黒 ( `B` ) か白 ( `W` ) のいずれかの色で塗ります． このとき，「各頂点の色（ `B` または `W` ）を頂点の番号順に並べて得られる文字列」を**色の列**と呼びます．

すべての頂点に色が塗られた状態で以下の操作を $ 1 $ 回行った結果として**あり得ない**色の列が存在するかどうかを判定し，存在するならそのような色の列を $ 1 $ つ求めてください．

**操作:** 各頂点 $ k\ =\ 1,\ 2,\ \dots,\ N $ に対して，辺で結ばれた頂点の色のうち過半数を占めるものを $ C_k $ とする． すべての頂点について同時に，頂点 $ k $ の色を $ C_k $ に塗り替える．

$ T $ 個のテストケースが与えられるので，それぞれについて答えてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ T $ $ \mathrm{case}_1 $ $ \mathrm{case}_2 $ $ \vdots $ $ \mathrm{case}_T $

各テストケース $ \mathrm{case}_i\ (1\ \leq\ i\ \leq\ T) $ は以下の形式である．

> $ N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ \vdots $ $ A_{\frac{3}{2}N} $ $ B_{\frac{3}{2}N} $

## 输出格式

$ T $ 行出力せよ． $ i $ 行目には，$ i $ 番目のテストケースについて，操作を行った結果としてあり得ない色の列が存在するならそのような色の列を，存在しないなら `-1` を出力せよ． 操作を行った結果としてあり得ない色の列が複数存在する場合，そのような色の列のうちどれを出力しても正答と見なされる．

## 输入输出样例 #1

### 输入 #1

```
2
4
1 2
1 3
1 4
2 3
2 4
3 4
10
1 2
1 3
1 4
2 3
2 4
3 5
4 5
5 6
6 7
6 8
7 9
7 10
8 9
8 10
9 10
```

### 输出 #1

```
BWWW
BWWWBWWWBB
```

## 说明/提示

### 制約

- $ T\ \geq\ 1 $
- $ N\ \geq\ 4 $
- $ 1 $ つの入力に含まれるテストケースについて，$ N $ の総和は $ 5\ \times\ 10^4 $ 以下である．
- $ N $ は**偶数**である．
- $ 1\ \leq\ A_i\ <\ B_i\ \leq\ N\ \left(1\ \leq\ i\ \leq\ \displaystyle\frac{3}{2}N\right) $
- $ (A_i,\ B_i)\ \neq\ (A_j,\ B_j)\ \left(1\ \leq\ i\ <\ j\ \leq\ \displaystyle\frac{3}{2}N\right) $
- 与えられるグラフは連結である．
- 各頂点 $ k\ (1\ \leq\ k\ \leq\ N) $ は $ A_i,\ B_i\ \left(1\ \leq\ i\ \leq\ \displaystyle\frac{3}{2}N\right) $ として**合計 $ 3 $ 回**現れる．
 
### Sample Explanation 1

$ 1 $ つ目のテストケースについて考えます． 頂点 $ 1 $ の色が `B` となるためには，操作を行う前に頂点 $ 2,\ 3,\ 4 $ のうち $ 2 $ つ以上の色が `B` である必要があります． このとき，頂点 $ 2,\ 3,\ 4 $ のうち少なくとも $ 1 $ つに関して，辺で結ばれた頂点のうち $ 2 $ つ以上の色が `B` であるため，操作を行った後の色は `B` となります． したがって，`BWWW` という色の列は操作を行った結果としてあり得ません．