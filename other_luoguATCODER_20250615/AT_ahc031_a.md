# AT_ahc031_a [AHC031A] Event Hall

## 题目描述

[problemUrl]: https://atcoder.jp/contests/ahc031/tasks/ahc031_a

縦横の長さが共に $ W $ のグリッドとして表現されるイベントホールがある。 一番左上の格子点の座標を $ (0,0) $ とし、そこから下方向に $ i $ マス、右方向に $ j $ マス進んだ先の格子点の座標を $ (i,j) $ とする。 一番右下の格子点の座標は $ (W,\ W) $ である。

$ D $ 日分の予約状況が与えられる。 各日の予約数は全て $ N $ であり、$ d=0,1,\cdots,D-1 $ 日目の $ k=0,1,\cdots,N-1 $ 番目の予約は面積 $ a_{d,k} $ 以上の長方形区画の貸出を希望している。 貸し出す長方形の形と位置は自由であるが、軸に平行かつ各頂点が格子点でなければならない。 また、同じ日の異なる2つの予約に対する長方形は正の面積の共通部分を持ってはならない。 貸し出されない空きスペースが残るのは構わない。

$ d $ 日目の $ k $ 番目の予約に対して貸し出す長方形区画を $ R_{d,k} $、その面積を $ b_{d,k} $ とする。 $ a_{d,k}\ >\ b_{d,k} $ の場合、$ 100\times\ (a_{d,k}-b_{d,k}) $ のコストが発生する。 $ a_{d,k}\leq\ b_{d,k} $ の場合にはコストは発生しない。

各長方形 $ R_{d,k} $ の外周のうち、グリッドの外周ではない部分にはパーティションを設置する必要があり、逆に、それ以外の場所にはパーティションが存在してはならない。 $ d $ 日目には、$ d-1 $ 日目のパーティションの配置から、この条件を満たすようにパーティションの設置・撤去を行う必要がある。 $ d $ 日目に設置・撤去を行ったパーティションの長さの合計が $ L_d $ のとき、$ L_d $ のコストが発生する。 ただし、**初日は特別に $ L_0=0 $ とする。**

より詳細には、$ L_d $ は以下のように計算される。 各 $ d=0,\cdots,D-1 $ に対して、グリッドの外周を除いた内部に含まれる横方向の各線分 $ (i,j)-(i,j+1) $ ($ 1\leq\ i\leq\ W-1,\ 0\leq\ j\leq\ W-1 $) がいずれかの $ R_{d,k} $ の外周上にある場合、 $ H_{d,i,j}=1 $、そうでない場合に $ H_{d,i,j}=0 $ と定義する。 この時、$ H_{d-1,i,j}\neq\ H_{d,i,j} $ であるような $ (i,j) $ 1つにつき、$ L_d $ に1が加算される。 同様に、縦方向の各線分 $ (i,j)-(i+1,j) $ ($ 0\leq\ i\leq\ W-1,\ 1\leq\ j\leq\ W-1 $) がいずれかの $ R_{d,k} $ の外周上にある場合、 $ V_{d,i,j}=1 $、そうでない場合に $ V_{d,i,j}=0 $ と定義する。 この時、$ V_{d-1,i,j}\neq\ V_{d,i,j} $ であるような $ (i,j) $ 1つにつき、$ L_d $ に1が加算される。

コストの合計が出来るだけ小さくなるように、貸し出す長方形区画を決定せよ。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ W $ $ D $ $ N $ $ a_{0,0} $ $ \cdots $ $ a_{0,N-1} $ $ \vdots $ $ a_{D-1,0} $ $ \cdots $ $ a_{D-1,N-1} $

- グリッドの縦横の長さ $ W $ は $ W=1000 $ で固定である。
- 日数 $ D $ は $ 5\leq\ D\leq\ 50 $ を満たす。
- 各日の予約数 $ N $ は $ 5\leq\ N\leq\ 50 $ を満たす。
- $ d $ 日目の $ k $ 番目の予約が希望する面積 $ a_{d,k} $ は $ 1\leq\ a_{d,0}\leq\ \cdots\leq\ a_{d,N-1} $ を満たす整数値であり、その和は $ a_{d,0}+\cdots+a_{d,N-1}\leq\ W^2 $ を満たす。

## 输出格式

$ d $ 日目の $ k $ 番目の予約に対して貸し出す長方形の左上の頂点の座標を $ (i_{d,k},j_{d,k}) $、右下の頂点の座標を $ (i_{d,k}',j_{d,k}') $ としたとき、 以下の形式で標準出力に出力せよ。

> $ i_{0,0} $ $ j_{0,0} $ $ i_{0,0}' $ $ j_{0,0}' $ $ \vdots $ $ i_{0,N-1} $ $ j_{0,N-1} $ $ i_{0,N-1}' $ $ j_{0,N-1}' $ $ \vdots $ $ i_{D-1,0} $ $ j_{D-1,0} $ $ i_{D-1,0}' $ $ j_{D-1,0}' $ $ \vdots $ $ i_{D-1,N-1} $ $ j_{D-1,N-1} $ $ i_{D-1,N-1}' $ $ j_{D-1,N-1}' $

各長方形は $ 0\leq\ i_{d,k}\lt\ i_{d,k}'\leq\ W $ と $ 0\leq\ j_{d,k}\lt\ j_{d,k}'\leq\ W $ を満たす必要がある。 この条件を満たさない場合、WA と判定される。

[例を見る](https://img.atcoder.jp/ahc031/PJcas1sL.html?lang=ja&seed=0&output=sample)

## 输入输出样例 #1

### 输入 #1

```
1000 5 10
6508 11666 12167 16717 46095 55928 56542 127260 200961 202211
11754 15667 26620 31851 48890 50181 52520 53150 263650 280526
7171 7218 14268 26231 37133 47199 93385 131356 174634 189807
10290 15811 16235 39805 45168 75830 76161 137648 148368 152504
6553 22994 44284 45120 67646 68899 98726 129109 138615 247097
```

### 输出 #1

```
0 43 23 326
747 654 824 843
863 2 1000 469
824 621 892 869
892 469 983 977
23 19 676 105
58 917 742 1000
494 398 747 917
85 105 863 398
6 398 403 911
166 917 329 1000
6 848 266 911
403 803 588 1000
863 633 983 977
361 19 494 398
361 398 494 803
494 105 588 767
863 0 1000 633
588 0 863 1000
0 19 361 848
10 740 81 841
949 196 1000 425
538 396 588 764
883 425 988 748
0 0 189 268
0 268 189 540
588 396 883 764
515 76 949 396
81 767 873 1000
189 0 515 583
363 460 538 767
363 767 600 923
762 767 873 923
288 923 807 1000
0 0 1000 76
188 397 363 832
10 376 188 841
0 76 462 376
515 76 949 425
538 425 988 764
10 376 86 736
288 452 330 1000
1 76 243 265
349 283 604 460
86 397 288 736
0 736 288 1000
243 8 604 283
330 520 600 1000
600 638 1000 1000
604 0 1000 638
```

## 说明/提示

### ストーリー

高橋くんはイベントホールの管理をしている。 このイベントホールは、パーティションを設置していくつかの長方形区画に区切ることが出来、各区画を別々の団体に貸し出している。

数日間の予約状況が与えられる。 各予約ごとに希望する区画の面積が指定されており、割り当てた区画の面積が指定された面積を下回った場合、コストが発生する。 また、区画の区切りを変更するためのパーティションの設置・撤去にも長さに応じたコストが発生する。 出来るだけコストの総和が小さくなるようにイベントホールを運営して欲しい。

### 得点

$ D $ 日間のコストの合計が $ C $ のとき、$ C+1 $ の絶対スコアが得られる。 **絶対スコアは小さければ小さいほど良い。**

各テストケース毎に、$ \mathrm{round}(10^9\times\ \frac{全参加者中の最小絶対スコア}{自身の絶対スコア}) $ の**相対評価スコア**が得られ、その和が提出の得点となる。

最終順位はコンテスト終了後に実施されるより多くの入力に対するシステムテストにおける得点で決定される。 暫定テスト、システムテストともに、一部のテストケースで不正な出力や制限時間超過をした場合、そのテストケースの相対評価スコアは0点となり、そのテストケースにおいては「全参加者中の最小絶対スコア」の計算から除外される。 システムテストは **CE 以外の結果を得た一番最後の提出**に対してのみ行われるため、最終的に提出する解答を間違えないよう注意せよ。

#### テストケース数

- 暫定テスト: 50個
- システムテスト: 2000個、コンテスト終了後に [seeds.txt](https://img.atcoder.jp/ahc031/seeds.txt) (sha256=16f021f46aad43a81ad05ebf38ed2b6ac813eafacbb6ad98549832218314db8f) を公開
 
#### 相対評価システムについて

暫定テスト、システムテストともに、CE 以外の結果を得た一番最後の提出のみが順位表に反映される。 相対評価スコアの計算に用いられる各テストケース毎の全参加者中の最小絶対スコアの算出においても、順位表に反映されている最終提出のみが用いられる。

順位表に表示されているスコアは相対評価スコアであり、新規提出があるたびに、相対評価スコアが再計算される。 一方、提出一覧から確認出来る各提出のスコアは各テストケース毎の絶対スコアをそのまま足し合わせたものであり、相対評価スコアは表示されない。 最新以外の提出の、現在の順位表における相対評価スコアを知るためには、再提出が必要である。 不正な出力や制限時間超過をした場合、提出一覧から確認出来るスコアは0となるが、順位表には正解したテストケースに対する相対スコアの和が表示されている。

#### 実行時間について

実行時間には多少のブレが生じます。 また、システムテストでは同時に大量の実行を行うため、暫定テストに比べて数%程度実行時間が伸びる現象が確認されています。 そのため、実行時間制限ギリギリの提出がシステムテストでTLEとなる可能性があります。 プログラム内で時間を計測して処理を打ち切るか、実行時間に余裕を持たせるようお願いします。

### サンプルプログラム

 Pythonでの解答例を示す。 このプログラムでは、$ k $ 番目の長方形として左上が $ (k,0) $、右下が $ (k+1,W) $ のものを出力している。

 ```
<pre class="prettyprint linenums">
# read input
W, D, N = map(int, input().split())
a = []
for d in range(D):
    a.append(list(map(int, input().split())))

# determine rectangles
rect = [[] for _ in range(D)]
for d in range(D):
    for k in range(N):
        rect[d].append((k, 0, k + 1, W))

# output
for d in range(D):
    for k in range(N):
        i0, j0, i1, j1 = rect[d][k]
        print(i0, j0, i1, j1)
```

### 入力生成方法

 $ L $ 以上 $ U $ 以下の整数値を一様ランダムに生成する関数を $ \mathrm{rand}(L,U) $ で表す。

日数 $ D $ は $ D=\mathrm{rand}(5,50) $ により生成される。 各日の予約数 $ N $ は $ N=\mathrm{rand}(5,50) $ により生成される。 パラメータ $ e $ を、$ e=\mathrm{rand}(500,5000)/10000 $ により生成し、平均空き面積 $ E $ を $ E=\mathrm{round}(W^2\ e^2) $ と設定する。 各 $ d=0,\cdots,D-1 $ に対し、以下のようにして $ a_{d,0},\cdots,a_{d,N-1} $ を生成する。

まず、$ T_d=\mathrm{rand}(W^2-\mathrm{floor}(\frac{3E}{2}),W^2-\mathrm{floor}(\frac{E}{2})) $ を生成する。 次に、集合 $ S=\{0,T_d\} $ から開始し、$ S $ の要素数が $ N+1 $ となるまで、$ \mathrm{rand}(1,T_d-1) $ を生成して $ S $ に追加する。 作成した集合 $ S $ の要素を小さい方から順に $ s_0(=0),s_1,\cdots,s_{N-1},s_N(=T_d) $ としたとき、 $ a_{d,k}=s_{k+1}-s_k $ と設定する。 最後に $ a_{d,0},\cdots,a_{d,N-1} $ を昇順に並び替える。

### ツール(入力ジェネレータ・ビジュアライザ)

- [Web版](https://img.atcoder.jp/ahc031/PJcas1sL.html?lang=ja): ローカル版より高性能でアニメーション表示が可能です。
- [ローカル版](https://img.atcoder.jp/ahc031/PJcas1sL.zip): 使用するには[Rust言語](https://www.rust-lang.org/ja)のコンパイル環境をご用意下さい。
  - [Windows用のコンパイル済みバイナリ](https://img.atcoder.jp/ahc031/PJcas1sL_windows.zip): Rust言語の環境構築が面倒な方は代わりにこちらをご利用下さい。
 
コンテスト期間中に、ビジュアライズ結果の共有や、解法・考察に関する言及は禁止されています。ご注意下さい。