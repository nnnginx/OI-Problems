# AT_ahc046_a [AHC046A] Skating with Blocks

## 题目描述

[problemUrl]: https://atcoder.jp/contests/ahc046/tasks/ahc046_a

$ N\ \times\ N $ のマス目からなるスケートリンクがある。 左上のマスの座標を $ (0,0) $ とし、下方向に $ i $ マス、右方向に $ j $ マス進んだ位置のマスの座標を $ (i,j) $ とする。 $ N\ \times\ N $ マスの外部はすべてブロックで覆われており、通過できない。 初期状態では、$ N\ \times\ N $ マスの内部にブロックは存在しない。

あなたは初期位置 $ (i_0,\ j_0) $ におり、指定された目的地 $ (i_1,\ j_1),\ \dots,\ (i_{M-1},\ j_{M-1}) $ をこの順番で訪れたい。

各ターンでは、上下左右のいずれかの方向を指定し、以下のいずれかの行動を 1 つ選んで実行できる。

- **移動**：指定した方向に隣接するマスへ 1 マス移動する。移動先がブロックであってはならない。
- **滑走**：指定した方向へ、ブロックにぶつかるまで直線的に滑走する。
- **変更**：指定した方向に隣接するマスに対し、ブロックが置かれていなければ設置し、すでに置かれていれば除去する。$ N\ \times\ N $ マスの外部は指定できない。なお、現在の目的地や将来の目的地にブロックを設置することも可能であるが、その場合、そのマスを訪れるにはブロックを除去する必要がある。
 
「滑走」によって目的地の上を通過した場合、そのマスを訪れたとはみなされない。目的地を訪れたと判定されるには、「移動」でそのマスに到達するか、「滑走」でそのマスに停止する必要がある。

目的地は指定された順番通りに訪れる必要がある。順番よりも後の目的地を先に通過しても、その時点では訪れたとはみなされない。順番が来たときに、あらためてそのマスを訪れる必要がある。

行動は最大 $ 2NM $ ターンまで行える。 出来る限り少ないターン数ですべての目的地を指定された順に訪れよ。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ i_0 $ $ j_0 $ $ \vdots $ $ i_{M-1} $ $ j_{M-1} $

- 全てのテストケースにおいて、$ N=20 $、$ M=40 $ に固定されている。
- 初期位置および目的地の座標 $ (i_k,\ j_k) $ は、$ 0\ \leq\ i_k,\ j_k\ \leq\ N-1 $ を満たす整数であり、すべて相異なる。

## 输出格式

各ターンに選択した行動と方向を、以下のようにアルファベット1文字ずつで表す。

**行動**

- 移動: `M`
- 滑走: `S`
- 変更: `A`
 
**方向**

- 上: `U`
- 下: `D`
- 左: `L`
- 右: `R`
 
$ t $ ターン目 ($ t\ =\ 0,\ 1,\ \dots,\ T\ -\ 1 $) の行動と方向をそれぞれ $ a_t $, $ d_t $ としたとき、以下の形式で標準出力に出力せよ。

> $ a_0 $ $ d_0 $ $ \vdots $ $ a_{T-1} $ $ d_{T-1} $

[例を見る](https://img.atcoder.jp/ahc046/EuNd3uow.html?lang=ja&seed=0&output=sample)

## 输入输出样例 #1

### 输入 #1

```
20 40
3 7
14 16
19 19
0 8
0 10
17 11
11 7
19 12
10 12
5 4
13 5
19 10
19 14
1 19
8 5
6 9
9 3
10 0
8 7
17 17
4 2
1 13
9 17
13 4
9 14
19 13
16 9
8 17
10 18
14 3
14 13
18 19
3 14
8 13
7 9
12 18
8 6
10 7
12 1
5 17
```

### 输出 #1

```
S D
M U
A D
M U
M U
M U
M U
S R
M L
M L
M L
S D
S R
S L
S U
M R
M R
```

## 说明/提示

### 得点

出力した行動列の長さを $ T $、訪れることが出来た目的地の数を $ m $ としたとき、以下のスコアが得られる。

- $ m\ <\ M-1 $ の場合、$ m+1 $
- $ m=M-1 $ の場合、$ M+2NM-T $
 
合計で 150 個のテストケースがあり、各テストケースの得点の合計が提出の得点となる。 一つ以上のテストケースで不正な出力や制限時間超過をした場合、提出全体の判定がWAやTLEとなる。 コンテスト時間中に得た最高得点で最終順位が決定され、コンテスト終了後のシステムテストは行われない。 同じ得点を複数の参加者が得た場合、提出時刻に関わらず同じ順位となる。

### 入力生成方法

初期位置および目的マスは、以下の手順に従って生成される。

まず、$ N^2 $ 個のすべてのマスの座標をランダムな順番に並び替える。 この並び替えた座標列のうち、先頭から $ M $ 個を順に $ (i_0,\ j_0),\ (i_1,\ j_1),\ \dots,\ (i_{M-1},\ j_{M-1}) $ として採用する。

### ツール(入力ジェネレータ・ビジュアライザ)

- [Web版](https://img.atcoder.jp/ahc046/EuNd3uow.html?lang=ja): ローカル版より高性能でアニメーション表示と手動プレイが可能です。
- [ローカル版](https://img.atcoder.jp/ahc046/EuNd3uow.zip): 使用するには[Rust言語](https://www.rust-lang.org/ja)のコンパイル環境をご用意下さい。
  - [Windows用のコンパイル済みバイナリ](https://img.atcoder.jp/ahc046/EuNd3uow_windows.zip): Rust言語の環境構築が面倒な方は代わりにこちらをご利用下さい。
 
コンテスト期間中に、ビジュアライズ結果の共有や、解法・考察に関する言及は禁止されています。ご注意下さい。