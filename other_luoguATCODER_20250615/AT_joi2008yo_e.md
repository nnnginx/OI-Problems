# AT_joi2008yo_e おせんべい

## 题目描述

[problemUrl]: https://atcoder.jp/contests/joi2008yo/tasks/joi2008yo_e

IOI 製菓では，創業以来の伝統の製法で煎餅（せんべい）を焼いている．この伝統の製法は，炭火で一定時間表側を焼き，表側が焼けると裏返して，炭火で一定時間裏側を焼くというものである．この伝統を守りつつ，煎餅を機械で焼いている．この機械は縦 $ R $ ($ 1\ \leqq\ R\ \leqq\ 10 $) 行，横 $ C $ ($ 1\ \leqq\ C\ \leqq\ 10000 $) 列の長方形状に煎餅を並べて焼く．通常は自動運転で，表側が焼けたら一斉に煎餅を裏返し裏側を焼く．

ある日，煎餅を焼いていると，煎餅を裏返す直前に地震が起こり何枚かの煎餅が裏返ってしまった．幸いなことに炭火の状態は適切なままであったが，これ以上表側を焼くと創業以来の伝統で定められている焼き時間を超えてしまい，煎餅の表側が焼けすぎて商品として出荷できなくなる．そこで，急いで機械をマニュアル操作に変更し，まだ裏返っていない煎餅だけを裏返そうとした．この機械は，横の行を何行か同時に裏返したり縦の列を何列か同時に裏返したりすることはできるが，残念なことに，煎餅を $ 1 $ 枚ごと裏返すことはできない．

裏返すのに時間がかかると，地震で裏返らなかった煎餅の表側が焼けすぎて商品として出荷できなくなるので，横の何行かを同時に $ 1 $ 回裏返し，引き続き，縦の何列かを同時に $ 1 $ 回裏返して，表側を焼きすぎずに両面を焼くことのできる煎餅，つまり，「出荷できる煎餅」の枚数をなるべく多くすることにした．横の行を $ 1 $ 行も裏返さない，あるいは，縦の列を $ 1 $ 列も裏返さない場合も考えることにする．出荷できる煎餅の枚数の最大値を出力するプログラムを書きなさい．

地震の直後に，煎餅が次の図のような状態になったとする．黒い丸が表側が焼ける状態を，白い丸が裏側が焼ける状態を表している．

![2008-yo-t5-1.png](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_joi2008yo_e/013dfdfbaa1335f538485984f0c741242dacee47.png)

$ 1 $ 行目を裏返すと次の図のような状態になる．

![2008-yo-t5-2.png](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_joi2008yo_e/1aaf6616b80a5085c22140cfbd2b1a9d93f6bdfa.png)

さらに，$ 1 $ 列目と $ 5 $ 列目を裏返すと次の図のような状態になる．この状態では，出荷できる煎餅は $ 9 $ 枚である．

![2008-yo-t5-3.png](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_joi2008yo_e/a352b3a75afa7349a79dec050f8630728b93d297.png)

## 输入格式

入力の $ 1 $ 行目には $ 2 $ つの整数 $ R,\ C $ ($ 1\ \leqq\ R\ \leqq\ 10,\ 1\ \leqq\ C\ \leqq\ 10\,000 $) が空白を区切りとして書かれている．続く $ R $ 行は地震直後の煎餅の状態を表す．($ i\ +\ 1 $) 行目 ($ 1\ \leqq\ i\ \leqq\ R $) には，$ C $ 個の整数 $ a_{i,1},\ a_{i,2},\ \ldots,\ a_{i,C} $ が空白を区切りとして書かれており，$ a_{i,j} $ は $ i $ 行 $ j $ 列 の煎餅の状態を表している. $ a_{i,j} $ が $ 1 $ なら表側が焼けることを，$ 0 $ なら裏側が焼けることを表す．

## 输出格式

出力は，出荷できる煎餅の最大枚数だけを含む $ 1 $ 行からなる．

- - - - - -

## 输入输出样例 #1

### 输入 #1

```
2 5
0 1 0 1 0
1 0 0 0 1
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
3 6
1 0 0 0 1 0
1 1 1 0 1 0
1 0 1 1 0 1
```

### 输出 #2

```
15
```

## 说明/提示

### ヒント

$ R $ の上限 $ 10 $ は $ C $ の上限 $ 10\,000 $ に比べて小さいことに注意せよ．

- - - - - -

### Sample Explanation 1

\- - - - - -