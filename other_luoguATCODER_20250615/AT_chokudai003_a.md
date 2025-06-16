# AT_chokudai003_a ○×ブロック

## 题目描述

[problemUrl]: https://atcoder.jp/contests/chokudai003/tasks/chokudai003_a

$ N $ × $ N $ の正方形のブロックが与えられます。 ブロックは、 `o`ブロック、 `x`ブロック、 `.`ブロックの $ 3 $ つが与えられています。

しばらくすると`.`ブロックが全て消滅し、上にあるブロックが落ちてくることを知っています。

あなたは、ブロックが消滅する前に、`.` ブロックを、以下の $ 2 $ 種類のブロックのどちらかに変換することが可能です。

- `+`ブロック：消滅しない普通のブロック
- `-`ブロック：消滅しないことに加え、自由落下もしないブロック

あなたは、書き換えた後に、`.`ブロック消滅後の、上下左右方向に連結する`o`ブロックの最大数と、同様に連結する`x`ブロックの最大数の和を できるだけ大きくしたいです。

ブロックを変更する前の状態が与えられるので、ブロックを変更した後の状態を出力してください。

## 输入格式

> $ S_1 $ $ S_2 $ : $ S_N $

## 输出格式

変更後のブロックの配置を、入力のフォーマットと同様の形で出力せよ。 ただし、`+`ブロックは`+`、`-`ブロックは`-`で表現するものとする。

連結数の和がそのケースの得点となり、 $ 10 $ 個の入力の点数の和が、あなたの提出の得点となる。

## 输入输出样例 #1

### 输入 #1

```
o.xx..ox..
..o.xx.o.x
.xxoo...o.
o..x.ox.x.
..o.o..ox.
..x..oo..x
.o.x.xxo..
x..xo.xxoo
.o..oox...
x.o.x.ox.x
```

### 输出 #1

```
o.xx..ox..
..o.xx.o.x
-xxoo...o.
o..x.ox.x.
..o.o+.ox.
..x..oo..x
.o.x.xxo..
x.+xo-xxoo
.o..oox+++
x.o.x.ox.x
```

## 输入输出样例 #2

### 输入 #2

```
.oo...x....xoo.xooooo.xx..xxo..xx.xoox.o..x..oo.o.
o..ox.xoxxox.xo..ooxx.ox.o.xooo.....x...ooxxo.o..x
x...x..oxxox.o..oxox.xoxo...oxo..oo....oxx.x...x.x
.xoo.........xo.xxx...x.o.xoox...o.o.x..ox.xx.oxo.
o.x...x.x.o.o...xo..oxxxo.xoo.xo.xo.ox.o...o...o..
xo.o.x..o.xx..o.....x..o.o....x.....ooo.oo.ooxx..o
.xx.o.xoo.x.xxx.x.o.xxoo.ox.o.oo.x.xxo..ox.x.o.o.o
.ox.o..xxo.ooxo.x.x.xx.xx.x...ooo.o..x....xo....ox
xx..ox.xx.x.x...ooxxox.oxx.o.oo.xo.o..x.x.xx..xxx.
o....o..x..xoxxx....o....x....x.o.o.x....ooo...o..
.xo.x...xox.............xo..xo....x..xoo.xx...x.ox
.oxxxxx.xx..o.oxoxx...x...x..x.oxxoxxo..oxx..xx...
.o..x.x.o...x..oo..o.x..xxox..o.oo.....x..x..o.oo.
ox.xo.xx.x..xo.oxooo..o.xxo.xox.o.x..xoo..o.x..oo.
.xoox...xoox...ooxx......o.oox....x.x.ox..o.ox.o.x
.o..x.xx..x....o..x.ox...oxooo....x..x.......o..x.
.o.xx..x..ox...o.o.xoo..oxx..oxo.oo..o.x.o.o....oo
x..xx.....x...o.xx.x..xo..x.oxx...xo.o...xx...xo.o
xx.oox.oxxo...ox...o.x..xo.oooxo..x..ox.ox...o...x
.oo...o.....o...xooxoxox.x.x...oo..xo.x.oo.x.xxxo.
oox..o.x.xo...oox.x..x..o.x.xxxo.x.x...o.o..o.....
xo.xx.o.x.xx.xo..oox..o..xoo...xo.o..ooo......oxox
.o..xx..xxo.....x...o.x..xxoxooxo..ooo.xx.....x..o
o..o.x..x.o.ox.oxx.o.xo.xox.o....o.o.x.ox...x.xox.
...o..oxoooo.x.o..oo....xo.xxxxxox..o.o.o....oo.o.
.xxo..x.x.oxoo.x.o....xxoxoo...ooxx.ox...ooo..x.x.
.xo..xxx.o..ox.oo....oox...xxo...oxx.o.ooo.o...oox
....ox.x.oo.o.x..x....o...o...x.oxx.oxo..o...oooo.
xxx..ox...x.x.x.o.x......xx..xx.ox.x......o.x..o.x
...oox.xox.ox.xx.x....x.oxxx..xxoxo.o.o....oxx...x
xoo.....ooxxxoxxxxx.....oxxx.....x..x...x..o.x..oo
..xo.oooxo...xx..x....x..oox.x.oxooo.oxoox...oxxo.
...ox.o.xo.oxxx....o..xooxox..x.xo...oo.xooo.x.xox
xx..o.oo...ox.x.x.ooxxxox...o..ox...ox....xx..xo..
xx.ooo..o.xoox.x.oox.o.xxxoooox.o..oo..x.x.xx....o
.oo...oxo.x.o.xx.o..xoxxox..x.xx.......xoxoxx.oxoo
...ox.ooooo.xxx.x..o.x.x.....xo..oo.xx..xo....ooox
.o.xx..o..xoxxo.xoo..xooo.xx.ox.xxxo.o.xo..o...x..
.xx...xoo.x.x.o.xo.o.xoxxo..oxo.ox....xoox.ox.xxxo
x.x..xox.....oxo..oo.ooxo...xo...ox.o..oo....ox.xo
.xx....xx.o....x.xoo.x.x.oxxooxxo..x..x..xxxxxo.ox
.o.x.x..x.oxoxx.xo..ox...ox.o......x.xxo...oo.oxx.
xx.xoxo.oo....ooxoxxxxxxxxoxxxx...oxx.o..oo.xo..xo
xx....o.o.xo.oox...o..o.x..o..x..x..xoxooxo.ox.oox
o.x..o.x..o.oo..ooo.x.......x.xx.o...oo..ox.x.xxx.
.xxoxoxxoo.o.o......xx..xxo.x....oox.x.xo.x..x....
oxx.oox....oxxx....x.oox..o.xx..xoxx.x.oo.o.o.x..x
....x.x.ox.xooxo.x..x.xo....oxoo..o.x.oo..o..x..x.
..o.o.xx....o...oooo...x.oox..oxox.x.x.x.xx...o.oo
..x.o.xo...xxx.x.ox.....oxo..ooxo..x.o.x..ooooxxox
```

### 输出 #2

```
.oo...x....xoo.xooooo.xx..xxo..xx.xoox.o..x..oo.o.
o..ox.xoxxox.xo..ooxx.ox.o.xooo.....x...ooxxo.o..x
x...x..oxxox.o..oxox.xoxo...oxo..oo....oxx.x...x.x
.xoo.........xo.xxx...x.o.xoox...o.o.x..ox.xx.oxo.
o.x...x.x.o.o...xo..oxxxo.xoo.xo.xo.ox.o...o...o..
xo.o.x..o.xx..o.....x..o.o....x.....ooo.oo.ooxx..o
.xx.o.xoo.x.xxx.x.o.xxoo.ox.o.oo.x.xxo..ox.x.o.o.o
.ox.o..xxo.ooxo.x.x.xx.xx.x...ooo.o..x....xo....ox
xx..ox.xx.x.x...ooxxox.oxx.o.oo.xo.o..x.x.xx..xxx.
o....o..x..xoxxx....o....x....x.o.o.x....ooo...o..
.xo.x...xox.............xo..xo....x..xoo.xx...x.ox
.oxxxxx.xx..o.oxoxx...x...x..x.oxxoxxo..oxx..xx...
.o..x.x.o...x..oo..o.x..xxox..o.oo.....x..x..o.oo.
ox.xo.xx.x..xo.oxooo..o.xxo.xox.o.x..xoo..o.x..oo.
.xoox...xoox...ooxx......o.oox....x.x.ox..o.ox.o.x
.o..x.xx..x....o..x.ox...oxooo....x..x.......o..x.
.o.xx..x..ox...o.o.xoo..oxx..oxo.oo..o.x.o.o....oo
x..xx.....x...o.xx.x..xo..x.oxx...xo.o...xx...xo.o
xx.oox.oxxo...ox...o.x..xo.oooxo..x..ox.ox...o...x
.oo...o.....o...xooxoxox.x.x...oo..xo.x.oo.x.xxxo.
oox..o.x.xo...oox.x..x..o.x.xxxo.x.x...o.o..o.....
xo.xx.o.x.xx.xo..oox..o..xoo...xo.o..ooo......oxox
.o..xx..xxo.....x...o.x..xxoxooxo..ooo.xx.....x..o
o..o.x..x.o.ox.oxx.o.xo.xox.o....o.o.x.ox...x.xox.
...o..oxoooo.x.o..oo....xo.xxxxxox..o.o.o....oo.o.
.xxo..x.x.oxoo.x.o....xxoxoo...ooxx.ox...ooo..x.x.
.xo..xxx.o..ox.oo....oox...xxo...oxx.o.ooo.o...oox
....ox.x.oo.o.x..x....o...o...x.oxx.oxo..o...oooo.
xxx..ox...x.x.x.o.x......xx..xx.ox.x......o.x..o.x
...oox.xox.ox.xx.x....x.oxxx..xxoxo.o.o....oxx...x
xoo.....ooxxxoxxxxx.....oxxx.....x..x...x..o.x..oo
..xo.oooxo...xx..x....x..oox.x.oxooo.oxoox...oxxo.
...ox.o.xo.oxxx....o..xooxox..x.xo...oo.xooo.x.xox
xx..o.oo...ox.x.x.ooxxxox...o..ox...ox....xx..xo..
xx.ooo..o.xoox.x.oox.o.xxxoooox.o..oo..x.x.xx....o
.oo...oxo.x.o.xx.o..xoxxox..x.xx.......xoxoxx.oxoo
...ox.ooooo.xxx.x..o.x.x.....xo..oo.xx..xo....ooox
.o.xx..o..xoxxo.xoo..xooo.xx.ox.xxxo.o.xo..o...x..
.xx...xoo.x.x.o.xo.o.xoxxo..oxo.ox....xoox.ox.xxxo
x.x..xox.....oxo..oo.ooxo...xo...ox.o..oo....ox.xo
.xx....xx.o....x.xoo.x.x.oxxooxxo..x..x..xxxxxo.ox
.o.x.x..x.oxoxx.xo..ox...ox.o......x.xxo...oo.oxx.
xx.xoxo.oo....ooxoxxxxxxxxoxxxx...oxx.o..oo.xo..xo
xx....o.o.xo.oox...o..o.x..o..x..x..xoxooxo.ox.oox
o.x..o.x..o.oo..ooo.x.......x.xx.o...oo..ox.x.xxx.
.xxoxoxxoo.o.o......xx..xxo.x....oox.x.xo.x..x....
oxx.oox....oxxx....x.oox..o.xx..xoxx.x.oo.o.o.x..x
....x.x.ox.xooxo.x..x.xo....oxoo..o.x.oo..o..x..x.
..o.o.xx....o...oooo...x.oox..oxox.x.x.x.xx...o.oo
..x.o.xo...xxx.x.ox.....oxo..ooxo..x.o.x..ooooxxox
```

## 说明/提示

### 制約

- $ N $ = $ 50 $
- $ S_i $ は $ N $ 文字の文字列であり、 $ j $ 番目の文字 $ S_{i,j} $ は、`o`,`x`,`.`の $ 3 $ 種類のどれかである。
- 入力は、各文字に対し、$ 50% $ の確率で `.`、残りの $ 25% $ の確率で`o`か`x`になるようにランダムで生成される。

### Sample Explanation 1

この入力は、説明のため、実際には存在しない小さい入力を使用しております。 全ての `.`ブロックが消滅したとき、以下のような状態になります。 図は、`o`ブロックを○、`x`ブロックを×、`+`ブロックを★、`-`ブロックを■で表現したものになります。 !\[例\](https://atcoder.jp/img/chokudai003/board.png)