# AT_genocon2021_c Practice 3

## 题目描述

[problemUrl]: https://atcoder.jp/contests/genocon2021/tasks/genocon2021_c

文字A, C, G, Tからなる$ m $本の文字列が与えられたとする．ここで，各文字列の適当な位置に空白を表す文字 - を挿入して長さを$ n $にそろえ，長さのそろった$ m $本の配列を$ m\ \times\ n $ の行列$ S $として表現する．$ S $の$ i $行目$ j $列の要素は$ S_{i,\ j} $と記述する $ (1\ \leq\ i\ \leq\ m,\ 1\ \leq\ j\ \leq\ n) $．また，行ベクトル，列ベクトルはそれぞれ$ S_{i,*} $, $ S_{*,j} $と記述する．ここで，- の挿入位置をうまく調節して，列ベクトルになるべく同じ文字をそろえたい．そこで，各々の列ベクトルがどの程度『そろっているか』を測るため，長さ$ m $の文字列$ t $に対して以下のスコア$ C $を定義する．

$ C(t)\ =\ min_{x\ \in\ \{A,\ T,\ G,\ C,\ -\}}\ \left|\ \{\ t[i]\ \;\ |\ \;\ t[i]\ \neq\ x\ \;\ (i=1,\ \ldots,\ m)\ \}\ \right| $

平たく言うと，$ C(t) $は$ t $に含まれる文字の中で最も出現回数の多い文字**以外**の文字の数となる．例えば，$ t $=CCCC-Tの場合，Cが最も多く出現するので，Cでない文字 - とTの総数を計算して$ C(t)=2 $となる．また，$ t $=CCAA-Tの場合，CとAが同率で最も多く出現するが，どちらを$ x $に選んでもスコアは変わらない．仮にCを選んだとすると，Cでない文字 A と - とTの総数を計算して$ C(t)=4 $となる．

$ S $のすべての列ベクトルについて$ C(S_{*,j}) $を計算し，その総和が少ないほど，同じ列に同じ文字が多く出現するように入力文字列をそろえることができていると言えるであろう．このように，文字列中の適切な場所に空白 - を挿入して三つ以上の文字列をそろえることをマルチプルアラインメントと呼ぶ．ここで，全ての列のスコアの総和を $ C_{all}(S)\ =\ \sum_{j=1}^n\ C(S_{*,j}) $ と定義する．

例えば，3本の文字列 GGATC, GGAT, GACCについて，以下のように各文字列に - を挿入してそろえると，

 ```
  GGATC
  GGAT-
  G-ACC
```

$ C_{all}(S)\ =\ C(S_{*,1})\ +\ C(S_{*,2})+\ C(S_{*,3})+\ C(S_{*,4})+\ C(S_{*,5})\ =\ 0\ +\ 1\ +\ 0\ +\ 1\ +\ 1\ =\ 3 $ となる．

$ m $本の文字列 $ s_{1},\ \ldots,\ s_{m} $ が与えられたとき，$ C_{all}(S) $をできるだけ小さくするマルチプルアラインメントを出力せよ．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ m $ $ s_{1} $ $ s_{2} $ : $ s_{m} $

## 输出格式

入力文字列について$ C_{all} $をできるだけ小さくするマルチプルアラインメントを出力せよ．例に倣い，各文字列の適切な位置に-を挿入した後，入力と同じ順序で出力すること． 全ての行は同じ長さでなければならない．また，各行の文字列から-を除いた文字列は，対応する入力文字列と一致していなければならない．

## 输入输出样例 #1

### 输入 #1

```
10
GGAGGTTATTGCTGTGGAGGTACTGGAGAAGGAGGATGCTAGCGTTGGGTAAACCACGAGCATTTTGACTTGTACTTCGCCTC
GGGTTATTGCTGTTGTGAGTACTGGAGACAGGAGGGAGTGTTAGAGTTGGGGTAAACCACAGTAGCTCATGTCACTTGGATAACTCGTCAGCCTC
GGTCACTCGCTGTGGAGAGTACTTTGAGACAGGAGGGAGTGCTAGAGTTTGGGGTAAAACCACAGCAGCTCATGCACTTGGATATCTGTGAGCC
GAGGTTAGTGCTGTGGAGAGTACTGGAGACAGGAGGGAGTGCTAGAGTTGGGGTAAAGCACAGCACCATTCACTGATAAATGTCAGGCCTAGGGG
GAGGTATTGCTGTGGAGGGTACTGGAGACAGGAGGAGTGCTAGAGGTTGGGGTAAAACCACAGCAGCTCATTTACTTGATACTGTCAGGCTCAGG
GAGGTTATTTGCTGTGGAGAGTTACTGAGACATGGGGTGCCAAGTTGGGTAGCTACAGCAGCTCATTTCACTTGATACTGCAGGCTCTCAG
GAGTTAATTTCGTGGAGAGTACTAGAGCACAGGAGGGAGGCCAGATTGGGGTATACCACAGCAGCTCGTTCACTTTAACTGTCAGGCCCTCA
ACAGTTTAATTGATGGGCGGAGAGTACTGGAGACAGGAGGGAGTGCTAGAGTGGGGTAAACCACAGCAGCATCTTTCATTATAACTGTCAG
CAAGGTTTTTTCGCTGTGGAGAGTACTGGAGACCGGGGAGTGTAGACTTTGGGGTATCACGTAGCAGCTTATTTCGACTTTGTACTGTAA
GAGTTATTTCTGTGGAGAGAACTGGAGACGGAGGGAGTGCTAGAGTTGGGGTAAACACCAGGCAGCCATTTCACTTGATAACTGTCAGGCCTT
```

### 输出 #1

```
GGAGGTTA-TTGCT--GTGGAG-GTAC-TGGAGA-AGGA-GGA-TGCTAGCG-TT-GGGT-AAACCAC-G-AGC-ATTTTGACTT-G-T-ACT--TC-GCCTC----
--GGGTTA-TTGCT--GTTGTGAGTAC-TGGAGACAGGAGGGAGTGTTAGAG-TTGGGGT-AAACCACAGTAGCTCATGTCACTTGGATAACTCGTCAGCCTC----
---GGTCACTCGCT--GTGGAGAGTACTTTGAGACAGGAGGGAGTGCTAGAGTTTGGGGTAAAACCACAGCAGCTCATG-CACTTGGATATCT-GTGAG-C-C----
-GAGGTTA-GTGCT--GTGGAGAGTAC-TGGAGACAGGAGGGAGTGCTAGAG-TTGGGGT-AAAGCACAGCA-CCATTCACTGATAAATGTCAGGCCTAGGGG----
--GAGGTA-TTGCT--GTGGAGGGTAC-TGGAGACAGGA-GGAGTGCTAGAGGTTGGGGTAAAACCACAGCAGCTCAT-TTACTT-GAT-ACT-GTCAGGCTC-AGG
-GAGGTTATTTGCT--GTGGAGAGTTACT-GAGACA--TGGG-GTGCCA-AG-TT-GGGT--AGCTACAGCAGCTCATTTCACTT-GAT-ACT-G-CAGGCTCTCAG
--GAGTTAATTTC---GTGGAGAGTACTAGAGCACAGGAGGGAG-GCCAGA--TTGGGGT-ATACCACAGCAGCTCGT-TCACTT---TAACT-GTCAGGC-CCTCA
ACAGTTTAATTGATGGGCGGAGAGTAC-TGGAGACAGGAGGGAGTGCTAGAG--TGGGGT-AAACCACAGCAGCATCTTTCA-TT--ATAACT-GTCAG--------
CAAGGTT-TTTTCGCTGTGGAGAGTAC-TGGAGAC-CG-GGGAGTG-TAGACTTTGGGGT---ATCAC-GTAG--CAGCTTATTTCG--ACTTTGT-A--CT-GTAA
--GAGTTA-TTTCT--GTGGAGAGAAC-TGGAGAC-GGAGGGAGTGCTAGAG-TTGGGGT-AAACACCAGGCAGCCATTTCACTT-GATAACT-GTCAGGC-C--TT
```

## 说明/提示

### 制約

- $ s_1 $,...,$ s_m $はA, C, G, Tからなる文字列である．
- テストケース（small）の場合
  - $ 8\ \leq\ m\ \leq\ 10 $とする．
  - $ 80\ \leq\ |s_1|,\ \ldots,\ |s_m|\ \leq\ 100 $ (文字列$ x $の長さを$ |x| $と記述する．)
- テストケース（large）の場合
  - $ 35\ \leq\ m\ \leq\ 40 $とする．
  - $ 700\ \leq\ |s_1|,\ \ldots,\ |s_m|\ \leq\ 750 $

### 配点

提出プログラムは「制約」の項目に記載した2種類のテストケース（smallとlarge）により評価される．smallに該当するケースは2つ，largeに該当するケースは8つ用意されている．制限時間内に正しい記述で出力された結果のみが評価の対象となる． smallの場合は各テストケースにつき，$ \{200\ -\ \lfloor\ C_{all}(S)\ *\ 0.2\ \rfloor\ \} $または0のいずれか大きい方の値が得点に加算される．largeの場合は，$ \{700\ -\ \lfloor\ C_{all}(S)\ *\ 0.1\ \rfloor\ \} $または0のいずれか大きい方の値が得点に加算される．例えば，制限時間内にsmallのケースのみ2つ回答できた場合は， $ max\{200\ -\ \lfloor\ C_{all}(S_1)\ *\ 0.2\ \rfloor,\ 0\}\ +\ max\{200\ -\ \lfloor\ C_{all}(S_2)\ *\ 0.2\ \rfloor,\ 0\} $が得点となる．（ただし，$ S_1 $, $ S_2 $はそれぞれのケースの出力．）

なお，最良の解が最大点（4500 6000点）に到達できることは保証しない．また，最終的な順位はコンテスト終了後に別のデータセットで評価する．現在ジャッジシステムに設置されているデータとコンテスト終了後に使用するデータセットは同じ方法で生成する．

### データ生成方法

参照ゲノム配列の一部（ヒトの22番染色体）から部分文字列$ s $を切り出す．ただし，A, T, G, C 以外の文字が含まれている領域は切り出しの対象としない．切り出した部分文字列に対して，シークエンサーの読み取りを模したエラー（挿入，欠損，置換）を発生させた文字列$ s' $を生成する．これを複数回繰り返して，一つのテストケースとする．なお，テストケースには$ s $は含まれない．どのようにしてシークエンサーの読み取りエラーを模したかは非公開とするが，テストデータセットは以下よりダウンロードできる．

- [テストケースダウンロード](https://waseda.box.com/s/k0hzpqdewytt1k8uqws03gqnvwouwaeb)

### 問題の背景

※ ***この項目は読まなくても問題を解くことができますが，出題の背景となりますため，ご興味を持ってくださった方はお読みいただけると幸いです．***

マルチプルアラインメントは，ペアワイズアラインメントと同様に，ゲノム配列解析の様々な場面において用いられます．ここでは，まず，ウィルスの変異解析について考えてみたいと思います．

ウィルスに感染すると，生体内ではウィルスのコピーがたくさん作られるのですが，その際，設計図となるDNAもしくはRNAも複製されます．しかし，複製の精度は100%ではないため，複製のたびに，新たに作られるウィルスのゲノムには様々な変異（置換，挿入，欠損など）が生じます．そのため，ゲノム配列が少しずつ異なるウィルスがたくさんできてしまうのです．このように少しずつ異なるけれど，大凡は似ている配列を比較して，変異の特徴を分析するのにマルチプルアライメントは役立ちます．

そのほかにも，シークエンサーから読み出された断片配列のエラー訂正にも使われます．DNAからゲノム配列を読み出す際には，シークエンサーのエラーを後で修正できるように，ゲノム上の同じ箇所を重複して読み取ります．こうして得られた断片配列には，読み出した際の状況に応じてエラーが含まれますが，これらの断片配列についてマルチプルアラインメントを作成して，各列について多数決をとれば，エラーを訂正することができます．