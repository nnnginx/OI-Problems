# AT_ahc041_a [AHC041A] Christmas Tree Cutting

## 题目描述

[problemUrl]: https://atcoder.jp/contests/ahc041/tasks/ahc041_a

$ N $ 頂点 $ M $ 辺の連結な無向平面グラフ $ G $ が与えられる。頂点には $ 0 $ から $ N-1 $ の番号が、辺には $ 0 $ から $ M-1 $ の番号がそれぞれ付けられている。頂点 $ v $ の座標は $ (x_v,\ y_v) $ であり、 辺 $ i $ は頂点 $ u_i $ と $ v_i $ を結んでいる。各頂点には正の整数をとる **美しさ** が定められており、頂点 $ v $ の **美しさ** は $ A_v $ である。

根付き木 $ T $ の **見栄え** を以下のように定義する。 $ T $ における頂点 $ v $ の **高さ** $ h_v $ を、根から $ v $ へのパスに含まれる辺の本数とする。 このとき、根付き木 $ T $ の **見栄え** $ a(T) $ は $ a(T):=\sum_{v\in\ T}\ (h_v\ +\ 1)\ A_v $ と定義される。

与えられたグラフ $ G $ から以下の条件を満たすような根付き木の集合を構築し、**見栄え** の総和をできるだけ大きくせよ。

- 各根付き木 $ T $ に含まれる辺は全て $ G $ に含まれる。
- $ G $ の各頂点はちょうど $ 1 $ つの根付き木に属する。
- 各根付き木における頂点の高さは全て $ H $ 以下である。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ H $ $ A_0 $ $ \cdots $ $ A_{N-1} $ $ u_0 $ $ v_0 $ $ \vdots $ $ u_{M-1} $ $ v_{M-1} $ $ x_0 $ $ y_0 $ $ \vdots $ $ x_{N-1} $ $ y_{N-1} $

入力は以下の制約を満たす。

- $ N=1000 $
- $ 1000\le\ M\ \le\ 3000 $
- $ H=10 $
- $ 1\le\ A_v\le\ 100 $
- $ 0\le\ u_i\ \lt\ v_i\le\ N-1 $
- $ 0\le\ x_v,\ y_v\le\ 1000 $
- $ (x_v,\ y_v) $ は全て異なる。
- 入力は全て整数。
- 与えられるグラフは連結な平面グラフであり、頂点 $ v $ を座標 $ (x_v,\ y_v) $ に配置し、各辺を両端点を結ぶ線分として描画した時、どの二辺も端点以外に共通点を持たないことが保証されている。

## 输出格式

構築した根付き木の集合における頂点 $ v $ の親の頂点番号を $ p_v $（$ v $ が根の場合は $ p_v=-1 $）として、以下の形式で標準出力に出力せよ。

> $ p_0 $ $ p_1 $ $ \cdots $ $ p_{N-1} $

[例を見る](https://img.atcoder.jp/ahc041/m0Bwp9WL.html?lang=ja&seed=0&output=sample)

解は複数回出力しても良い。 複数出力された場合、一番最後に出力された解のみが採点に用いられる。 Web版のビジュアライザを用いると、複数の解の比較が可能である。

## 说明/提示

### ストーリー

AtCoderオフィスでは、一足遅いクリスマスパーティーの準備が進められている。高橋社長は、クリスマスツリーに使う根付き木を切りに行くことにした。

根付き木の各頂点は **美しさ** を持ち、高いところに美しい頂点が存在するとパーティー会場の **見栄え** が良くなる。ただし、根付き木が高すぎるとAtCoderオフィスの天井にぶつかってしまうため、パーティー会場に持ち込むことのできる根付き木の高さには制限がかけられている。

与えられたグラフから根付き木をいくつか切り出して、できるだけパーティー会場の **見栄え** を良くして欲しい。

### 得点

出力した根付き木の集合を $ F $ としたとき、$ 1+\sum_{T\in\ F}a(T) $ の得点が得られる。

合計で 150 個のテストケースがあり、各テストケースの得点の合計が提出の得点となる。 一つ以上のテストケースで不正な出力や制限時間超過をした場合、提出全体の判定がWAやTLEとなる。 コンテスト時間中に得た最高得点で最終順位が決定され、コンテスト終了後のシステムテストは行われない。 同じ得点を複数の参加者が得た場合、提出時刻に関わらず同じ順位となる。

### 入力生成方法

$ L $ 以上 $ U $ 以下の整数値を一様ランダムに生成する関数を $ \mathrm{rand}(L,U) $ と表す。

#### グラフ $ G $ の生成

中心 $ (500,500) $ 、半径 $ 500 $ の円に含まれる格子点からランダムに点を一つずつ、合計 $ N $ 個選んで $ (x_0,\ y_0),\ \cdots,\ (x_{N-1},\ y_{N-1}) $ とする。ただし、既に選んだ点とのユークリッド距離が $ 15 $ 以下の場合は選び直す。

以上により得られた頂点集合 $ V $ に対して[ドロネー三角形分割](https://ja.wikipedia.org/wiki/%E3%83%89%E3%83%AD%E3%83%8D%E3%83%BC%E5%9B%B3)を計算し、三角形分割の辺集合を $ E $ として $ G=(V,\ E) $ とする。

#### 美しさ $ A $ の生成

頂点 $ v $ の美しさは $ A_v=\mathrm{rand}(1,\ 100) $ により生成する。

### ツール(入力ジェネレータ・ローカルテスタ・ビジュアライザ)

- [Web版](https://img.atcoder.jp/ahc041/m0Bwp9WL.html?lang=ja): ローカル版より高性能でアニメーション表示が可能です。
- [ローカル版](https://img.atcoder.jp/ahc041/m0Bwp9WL.zip): 使用するには[Rust言語](https://www.rust-lang.org/ja)のコンパイル環境をご用意下さい。
- [Windows用のコンパイル済みバイナリ](https://img.atcoder.jp/ahc041/m0Bwp9WL_windows.zip): Rust言語の環境構築が面倒な方は代わりにこちらをご利用下さい。
 
コンテスト期間中における、ビジュアライズ結果の共有や解法・考察に関する言及は禁止されています。ご注意下さい。