# AT_yuha_c83_01 Revenge of Voronoi - ボロノイの逆襲

## 题目描述

[problemUrl]: https://atcoder.jp/contests/yuha-c83/tasks/yuha_c83_01

「離散ボロノイ図」はボロノイ図の亜種である。 離散ボロノイ図では、図は画素の集合として表現される。 各母点はいくつかの画素の中心に位置しており、 各画素はマンハッタン距離で最も近い母点に所属している。 ここでマンハッタン距離は2つの点 $ (x_{1},\ y_{1}) $ と $ (x_{2},\ y_{2}) $ に対して 以下の式で与えられる距離である。 あなたの仕事は与えられた離散ボロノイ図に対し、 各母点の座標を計算するプログラムを書くことである。 与えられる離散ボロノイ図において、各母点は他の母点と重複しない英小文字で表される。 また各画素は、その点が所属する母点の文字で表される。 一つの画素が複数の母点から等距離にある場合は、 その画素は等距離にある母点のうち、 最も若い英小文字で表される母点に所属する。 入力の1行目には二つの整数、 $ W\ (1\ <\ =\ W\ <\ =\ 50) $ と $ H\ (1\ <\ =\ H\ <\ =\ 50) $ からなり、 それぞれ離散ボロノイ図の幅と高さを表す。 続く $ H $ 行には、 $ W $ 文字の英小文字が含まれており、 各文字が一つの画素を表す。 サンプル出力に示されている通りに母点の座標を出力せよ。 各行は母点を表す英小文字、X座標、Y座標からなる。 母点はそれぞれを表す英小文字のアルファベット順で出力せよ。 座標は $ (0,0) $ を左上の画素の中心とする。 各テストケースにつき、少なくともひとつは解が存在すると仮定して良い。 また、複数の解が存在する場合は、いずれを出力しても構わない。

- $ 1\ <\ =\ W,\ H\ <\ =\ 8 $ を満たす入力にのみ正解した場合、部分点として $ 50 $ 点が与えられます
- $ 1\ <\ =\ W,\ H\ <\ =\ 16 $ を満たす入力にのみ正解した場合、部分点として $ 50 $ 点が与えられます
 
```
4 3
ooxx
ooxx
ooxx
```

 ```
o 0 0
x 2 0
```

 ```
4 1
null
```

 ```
l 2 0
n 0 0
u 1 0
```

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_yuha_c83_01/fb8ebb190e14f0f45b61cb7cdf954b7f5f43506b.png)

 ```
4 4
aabb
aabb
ccdd
ccdd
```

 ```
a 0 0
b 2 0
c 0 2
d 2 2
```

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_yuha_c83_01/01e19d15f00f3474d5c19fdf660f794f19b23cee.png)

## 输入格式

无

## 输出格式

无