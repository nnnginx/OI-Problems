# AT_code_formula_2014_final_g ノイハの塔

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-formula-2014-final/tasks/code_formula_2014_final_g

「ハノイの塔」という有名なパズルがあります。 ハノイの塔は $ 3 $ つの杭と、中央に穴の空いたサイズが相異なる $ N $ 個の円盤からなるパズルです。 $ 3 $ つの杭には $ 1 $ から $ 3 $ の番号が付けられています。また、 $ i $ 番目に小さい円盤の半径は $ i $ センチメートルです。

初め、全ての円盤は杭 $ 1 $ に、サイズが大きい順に下から積み重ねられて、「塔」を形成しています。杭 $ 2,\ 3 $ には何も置いていません。 プレイヤーは $ 1 $ 回の操作で、ある杭の塔の一番上にある円盤を、他の杭に移動させて、移動先の杭の塔の一番上に積み重ねるという事ができます。 このとき、小さい円盤の上に大きい円盤を置くことはできません。 ハノイの塔のゴールはできるだけ少ない回数の操作で、高さ$ N $の塔を杭 $ 2 $ もしくは杭 $ 3 $ に移すことです。

高橋君は久しぶりにこのパズルを遊ぼうと思い、押し入れの奥からハノイの塔のおもちゃを探しだしました。 しかし、だれかがいたずらをしたようで、$ N $ 個全ての円盤がバラバラの順番で杭 $ 1 $ に積まれていました。 そこで高橋君はそのバラバラの状態から開始して、「小さい円盤の上に大きい円盤を置いてはならない」というルールを無視して操作し、いずれかの杭に全ての円盤がサイズが大きい順に下から積み重なるように移動させる、という別のパズルを遊ぶことにしました。

あらかじめ、杭 $ 1 $ に積み重ねられている円盤のサイズの情報が与えられるので、いずれかの杭(杭 $ 1 $ でもよい)に全ての円盤がサイズ順に積み重なるように移動させる操作をひとつ挙げてください。 ただし操作が多すぎるとパズルとして美しくないので $ 225,000 $ 回以内の操作で移動させてください。

## 输入格式

入力は以下の形式で標準入力から与えられる

> $ N $ $ r_1 $ $ r_2 $ : $ r_N $

- $ 1 $ 行目には円盤の個数 $ N\ (1\ ≦\ N\ ≦\ 10,000) $ が与えられる。
- $ 2 $ 行目からの $ N $ 行のうち $ i $ 行目には、初め杭 $ 1 $ に下から $ i $ 番目に置かれている円盤の半径 $ r_i\ (1\ ≦\ r_i\ ≦\ N) $が与えられる。
- $ x\ ≠\ y $ ならば $ r_x\ ≠\ r_y $ が成り立つ。

## 输出格式

出力形式は以下のようなものである。

> $ M $ $ from_1 $ $ to_1 $ $ from_2 $ $ to_2 $ : $ from_M $ $ to_M $

- $ 1 $ 行目には操作の回数 $ M $ を出力せよ。
- $ 2 $ 行目からの $ M $ 行のうち $ i $ 行目には$ i $番目の操作で動かす円盤の元あった杭の番号 $ from_i $ と動かす先の杭の番号 $ to_i $ を空白区切りで出力せよ。
- $ i $ 番目の操作の時に、杭 $ from_i $ に円盤が一つも存在しない場合、その操作は妥当でないとする。それ以外の操作は妥当であるとする。
- 本来のハノイの塔と異なり小さい円盤の上に大きい円盤を置くことが許されていることに注意せよ。
- $ M\ ≦\ 225,000 $ かつすべての操作が妥当であり、最後にいずれかの杭に全ての円盤がサイズの大きい順に下から積み重ねられていたときのみ、解答は正解とされる。

## 输入输出样例 #1

### 输入 #1

```
5
1
2
3
4
5
```

### 输出 #1

```
5
1 2
1 2
1 2
1 2
1 2
```

## 输入输出样例 #2

### 输入 #2

```
5
5
3
2
4
1
```

### 输出 #2

```
8
1 2
1 2
1 3
1 3
2 1
3 1
3 1
2 1
```

## 说明/提示

### 部分点

この問題には部分点が設定されている。

- $ 1\ ≦\ N\ ≦\ 400 $を満たすデータセットに正解した場合は $ 30 $ 点が与えられる。
- $ 1\ ≦\ N\ ≦\ 10,000 $を満たすデータセットに正解した場合はさらに $ 70 $ 点が与えられる。合計で$ 100 $点となる。

### Sample Explanation 1

初め、全ての円盤が逆順に杭 $ 1 $ に積み重ねられています。上から順番に杭 $ 2 $ に移動させれば、下から大きい順に並び替えられます。

### Sample Explanation 2

最後に全ての円盤が積み重ねられる杭は $ 1 $ でもかまいません。