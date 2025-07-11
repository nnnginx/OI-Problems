# AT_genocon2021_d Mind the Difference

## 题目描述

[problemUrl]: https://atcoder.jp/contests/genocon2021/tasks/genocon2021_d

文字A, C, G, Tからなる $ 2 $ 本の秘密文字列 $ s_1,\ s_2 $ が存在する．$ s_1,\ s_2 $ は多くの場合には 99% 以上一致しているが, 大きく異なる場合もある． $ s_1,\ s_2 $ の長さをそれぞれ $ l_1,\ l_2 $ とする．２本の秘密文字列に対して以下のような観測や操作を行った結果として $ B $ が与えられる．$ B $ の情報を利用して秘密文字列を推測し，$ s_1,\ s_2 $ としてなるべく確からしい文字列２本を出力せよ．

(1) 観測は以下の「観測試行」を$ n $ 回繰り返すことで行われ， $ n $ 本の文字列を得る．

(2) 観測試行で得られた $ n $ 本の文字列に対して以下の操作を行う．

(2a) $ s_1,\ s_2 $ と似ている（と出題者が考えている）配列 $ r $ が存在する． この配列 $ r $ と観測試行で得られた $ n $ 本の文字列をそれぞれペアワイズアラインメント（ペアワイズアラインメントの定義は問題Bを参照）する

(2b) ペアワイズアラインメントの結果（$ n $ 個）と $ r $ を合わせて結果 $ B $ とする．結果 $ B $ に含まれる $ n $ 個のペアワイズアラインメントは全て配列 $ r $ と同じ向きに揃えられている．

#### 観測試行

(1) $ s_1 $ と $ s_2 $ のどちらかをそれぞれ 50% の確率で選択し，選択した文字列を $ s_i $ とする．

(2) 選択した文字列$ s_i $に対して始点の座標$ b $ を一様ランダム $ (-l_i\ \le\ b\ \le\ l_i) $ に, 終点の座標 $ e $ を $ e\ -\ b $ がある分布に従うように決める． $ e $ が $ 0 $ 以下となった場合には観測試行を (1) からやり直す．

(3) $ b $ が $ 1 $ 以下である場合には $ b $ に $ 1 $ を代入する． $ e $ が $ l_i $ より大きい場合には $ e $ に $ l_i $ を代入する．

(4) $ t\ =\ s_i\ [b:\ e] $ （$ s_i $ の $ b $ 文字目から $ e $ 文字目）と置く．

(5) 50% の確率で $ t $ に $ t $ の逆相補鎖（逆相補鎖問題の定義はＡ参照）を代入する． 代入したときには $ f\ = $&lt;, そうでないときには $ f\ = $&gt; とする．$ f= $&lt; の場合であっても最終的な結果 $ B $ に含まれるペアワイズアラインメントは $ r $ と同じ向きに揃えられていることに注意せよ．ただし，$ B $ には各文字列がもともとどちらの向きであったかを示す情報（すなわち $ f $ ）が含まれている．

(6) $ t $ を観測して$ f $ と文字列を出力する． 文字列観測の際にはエラーが発生する． エラーの種類には, 文字が別の文字に置き換わってしまう**置換**, 文字が増減する**挿入**や**欠失**がある． 詳しくは**観測エラーについての補足**を参照のこと．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ g $ $ f_{1} $ $ r_{1} $ $ c_{1} $ $ f_{2} $ $ r_{2} $ $ c_{2} $ : $ f_{n} $ $ r_{n} $ $ c_{n} $ =

観測した DNA の断片配列が $ n $ 本与えられるが，入力データサイズを節約するために $ n $ 本の配列は圧縮表記で与えられ，標準的な DNA 配列とそこからの差分という形式で与えられる．入力1行目の $ g $ は標準的な DNA 配列であり，$ 1 $ 文字以上 $ 101,000 $ 文字以下の文字列である．

続いて入力の $ 2 $ 行目以降を説明する．$ 2 $ 行目から$ n+1 $ 行目では 1 行につき 1 本の観測したDNA断片配列が記述される．各行最初の $ f_i $ は参照配列に対する DNA の向きを与える．DNA の向きは右向き（$ g $ と同じ向き）の場合には &gt; を，左向き（$ g $ の逆相補鎖の向き）の場合には &lt; が与えられている．この情報は使わなくても本問題は一定程度解けるが，DNA の向きによってエラーの傾向が異なることが分かっているため，この情報を積極的に用いることでスコアを向上させることが可能であると見込まれている． $ r_{i},\ c_{i} $ のペアは観測した DNA 断片配列を圧縮した形で表す．具体的には $ g $ の一部分を元に差分を表現している．最初に，$ g $ の $ r_i $ 文字目（$ r_i $ は 0-origin であり，最初の文字は $ 0 $ 文字目である）にカーソルを置く．$ c_i $ は｛長さ｝｛タイプ｝｛補助情報｝ の３つ組を０個以上反復して連結した文字列である．｛長さ｝は任意長の数字で表され，｛タイプ｝は１文字である．｛補助情報｝は｛タイプ｝の種類により存在しない場合も存在する場合もあるが，補助情報が存在する場合には｛補助情報｝は｛長さ｝で指定される長さの文字列であり，そうでない場合には｛補助情報｝は空文字列である．

「タイプ」には参照ゲノム配列との**一致**を表す=と**不一致**を表す X ，そして参照配列からの**欠失**を表す D，参照配列からの**挿入**を表す I の４タイプがある．

入力の終端は = のみを含む行で与えられる．（$ n $ は = が現れるまでの行数として暗黙のうちに与えられる）

「タイプ」について詳細を説明するため，**一致**，**不一致**，**欠失**，**挿入**それぞれについて，以下で具体例を示す．

#### 一致の例

観測試行回数 $ n=1 $ の例を使って**一致**を説明する．以下に示すのは1 本の配列だけを入力とする入力例とそれに対応する１本の観測配列である．

 ```
ACGTGCTTA
> 0 6=
=
```

 ```
ACGTGC
```

6= は標準ゲノム上にある現在カーソル位置から 6 文字を取得して出力する命令である．$ r=0 $ であり，カーソルは左端にあるため，$ g $ の先頭から 6 文字が取得され，ACGTGC が出力として得られた．

もう１つの入力例とそれに対応する１本の観測配列を示す．

 ```
ACGTGCTTA
< 2 4=
=
```

 ```
GTGC
```

この例は初期カーソル位置を変えた例となっている．先頭から 2 文字スキップした位置がカーソル位置であり，そこから 4 文字を出力し GTGC が出力される．一致が発生した場合には出力した文字数だけカーソル位置を右にずらす．

以下の入力例では 2= と 3= を繋げているが，これは5= と同じ意味となり，カーソル位置から 5 文字（2+3文字） をコピーして出力する．結果として観測配列は CGTGC となる．

 ```
ACGTGCTTA
< 1 2=3=
=
```

 ```
CGTGC
```

#### 不一致の例

標準ゲノムとは異なる文字を出力する場合にはタイプ X を用いる．｛長さ｝X｛内容｝ という文字列が与えられた場合には，｛内容｝ を出力し，カーソルを長さの分だけ右に進める．以下の入力例では

 ```
ACGTGCTTA
> 0 3=2XGA4=
=
```

3=（３文字**一致**）と2XGA（２文字 GA を出力し２文字カーソルを進める）と4=４文字**一致**を連続して実行し，観測配列としては以下の文字列を表している．

 ```
ACGGACTTA
```

対応関係を見やすく書くと，以下のようになる．標準ゲノムを $ g $ とし，観測配列を $ A $ として示した．見やすさ一のために，一致する文字の間に | を，不一致の文字の間に X を記した．

 ```
g: ACGTGCTTA
   |||XX||||
A: ACGGACTTA
```

#### 欠失の例

標準ゲノムに対して欠失がある場合にはタイプ D を用いる．｛長さ｝D という文字列が与えられた場合には何も出力せずにカーソルを長さの分だけ右に進める．以下の入力例では座標 1 （先頭から１文字スキップした場所）から 2= （２文字一致）, 1D （１文字欠失（削除）），4=（４文字一致）させている．

 ```
ACGTGCTTA
< 1 2=1D4=
=
```

 ```
CGGCTT
```

この観測配列 $ A $ と標準ゲノム $ g $ の対応関係を見やすく書くと以下のようになる．一致する文字が縦に並ぶ方が見やすいため観測配列 $ A $ に - を挿入して桁をずらしている．

 ```
g: ACGTGCTTA
    || ||||
A:  CG-GCTT
```

#### 挿入の例

標準ゲノムに対して挿入がある場合にはタイプ I を用いる． ｛長さ｝I｛内容｝ という文字列が与えられた場合にはカーソルを進めずに｛内容｝を出力する．以下の入力例では座標 2（先頭から２文字スキップした場所）から 2= （２文字一致）, 2IAT （２文字ATを挿入），3=（３文字一致）させており，入力例とそれに対応する観測配列は以下のようになる．

 ```
ACGTGCTTAG
> 2 2=2IAT3=
=
```

 ```
GTATGCT
```

同様に標準ゲノム $ g $ と観測配列 $ A $ の対応関係を見やすく書くと以下のようになる．一致する文字が縦に並ぶ方が見やすいため $ g $ に - を挿入して表示している．

 ```
g: ACGT--GCTTAG
     ||  |||
A:   GTATGCT
```

#### 圧縮表記に関する補足

標準的なDNA配列と$ n $ 本の観測文字列の間の対応関係は，ゲノム業界で標準的なツールの１つを使って計算されているため，多くの場合には配列間の関係は正しいと考えられる．しかし，対応関係が間違っている場所もあることに注意されたい．例えば以下の例において，標準ゲノム $ g $ と観測対象のゲノム $ T $ の間の真の対応関係（神が存在してDNAシークエンサーの観測エラーがどのように発生したかが分かり，真に対応する文字を上下に並べた場合）が以下のようになっていた場合であっても, 観測配列$ A $ のような誤った対応関係が出力されていることがある．

 ```
g: ACGTGCGTAGCG
   |||  |  ||||
T: ACG--C--AGCG
   |||     ||||
A: ACGC----AGCG
```

このような並べ間違いは入力中に多く含まれているがこのような間違いを修正することでスコアを向上させることができる可能性がある．

また，圧縮表記の取り扱いはコンテストの主眼ではないため，参加者にとってデバッグが容易になるように Python で圧縮表記からマルチプルアラインメント（マルチプルアラインメントについては問題Ｃを参照のこと）を生成する [Python 3 向けのサンプルコード](https://iibmp2021.hamadalab.com/genocon/decode_cigar.py) を用意した．第一引数に本問題の入力データ例のファイルを与えるとテキスト表記のマルチプルアラインメントを出力する．

## 输出格式

推測した２本の秘密配列を２行に分け，１行に１配列ずつ出力する．出力する配列には A, C, G, T 以外の文字が含まれていてはならない．また，２行目の終端は必ず改行すること．

## 输入输出样例 #1

### 输入 #1

```
ACACAGCGGCGACC
> 0 3=1XT10=
< 0 14=
< 0 9=1D4=
< 0 14=
< 0 14=
< 0 9=1D4=
=
```

### 输出 #1

```
ACACAGCGGCGACCT
ACATAGCGGGACT
```

## 输入输出样例 #2

### 输入 #2

```
ACCGGTTGGCGTG
> 0 5=
< 1 8=
> 2 2=1XA3=1IC3=
< 4 5=1D2=
> 7 6=
=
```

### 输出 #2

```
ACCGGTTGGCGTG
ACCGGTTGGCGTG
```

## 说明/提示

### 更新履歴

- 28th September, 2021 (JST): **コンテスト終了に伴い，テストケースを削除しました．また，サンプルデータの配布も終了しました．D問題は，問題文のみの公開となります．プログラムを提出してもジャッジは行われません．コンテスト開催時の実行時間制限は30秒でした．**
- 11th September, 2021 (JST): サンプルデータのダウンロードに必要な情報を追記しました．
- 10th September, 2021 (JST): Sample2 終端記号が抜けているのを直しました. 本文中の f = 0 という誤りを f = &gt; に修正しました．ダウンロードできるサンプルデータに - や X が含まれる理由の解説を加えました．
- 9th September, 2021 (JST): ダウンロードデータセットに関する注意書きを追加しました．
- 9th September, 2021 (JST): 日本語の問題文を公開しました．ジャッジサーバーが動いています．

### 追加情報（トップページより転載）

- 2021/9/12 : D問題に関しまして，Dockerによる手元ジャッジ環境を準備しました．[**こちら(GitHub)**](https://github.com/exKAZUu/genocon2021-docker)よりダウンロードできます．手元でのジャッジの他，入力のパース，非常に基本的な解を出力するプログラムも含まれております．
- 2021/9/12 : D問題に関しまして，BAM形式のビューア―の使い方を記載した資料を準備しました．[**こちら**](https://iibmp2021.hamadalab.com/genocon/how_to_use_IGV.pdf)からダウンロード頂けます．

### ストーリー

あなたは Oxford Nanopore Technologies 社の最新機器である PromethION を手に入れた！PromethION は DNA を読み取る機械である．この機械を用いてあなたは自分の DNA 配列を解析しようと試みた．しかし，PromethION はあなたの DNA 配列を端から端まで100%正確に読み取れるわけではない．PromethION に投入するために DNA を精製すると，DNA は千切れてバラバラになってしまう．このため，１回の観測で得られる配列はDNA 配列の一部分だけだ．また，観測エラーもあるため，読み取ったDNA配列の断片配列の集合からあなたのDNA配列を精密に予測することは簡単ではない．あなたのミッションは，PromethION の出力データからあなたの真の DNA 配列を推測することである．あなたの DNA 配列には父から受け継いだ配列と母から受け継いだ配列の２本があり，２本ともなるべく正確に推測したい．

### くだけた問題の説明

![](https://iibmp2021.hamadalab.com/genocon/prob_d_picture/informal_pd.png)

実際の観測試行では始点の座標と終点の座標がバラバラであり，n 本の観測試行を重ねて表示したものを縮小して表示した一例を以下に示す．A, C, G, T がそれぞれ異なる色に割り当てられており，スペース節約のために観測試行はなるべく上に詰めて表示している．また，各観測試行の端にグレーの三角印が付いているが観測試行の向き $ f $ を表している．大きな欠失は細い水平の黒線で表されており，挿入は潰れて認識しにくく表示されている．

![](https://iibmp2021.hamadalab.com/genocon/prob_d_picture/informal_pd2.png)

### 観測エラーについての補足

観測エラーは置換，挿入，欠失の３種類からなる．観測エラーはシミュレーションではなく実機の PromethION と開発中の試薬を用いることで結果として含まれているため，どのような時にどれぐらいの頻度でどのようなエラーが入るかは出題者にも厳密には分からない．観測エラーの性質を分析できるように，既知の DNA 配列を PromethION で読んだデータが別途ダウンロード可能である（後述）．

#### 置換

ある文字が別の文字に置き換わる．以下の例では２文字目の C が G に置き換わってしまっている．

 ```
元文字列　: ACCAG
観測文字列: AGCAG
```

#### 挿入

元文字列には存在しない配列（任意長）が観測文字列に追加される．以下の例では元文字列の２文字目と３文字目の間に AA が挿入されている．

 ```
元文字列　: ACGAG
観測文字列: ACAAGAG
```

#### 欠失

元文字列に存在する配列（任意長）が観測文字列に現れない．以下の例では元文字列の３文字目に存在する G が観測文字列上で無くなっている．

 ```
元文字列　： ACGAG
観測文字列： ACAG
```

### 制約

- $ s_1,\ s_2 $はA, C, G, Tからなる文字列である．
- $ 3\ \leq\ l_1,\ l_2\ \leq\ 101,000 $とする．
- $ n\ \le\ 200 $ である

### スコア

出力された２本の配列を $ o_1,\ o_2 $ とする． もし $ o_1,\ o_2 $ を入れ替えた場合にスコアが上がる場合には入れ替えたうえでスコアを計算する．

$ o_1 $ と $ s_1 $, $ o_2 $ と $ s_2 $ を比較し, 1 文字正解するごとに $ 0.01 $ 点が与えられる． 1 文字不正解（１文字の置換・１文字の欠失・１文字の挿入）するごとに $ 0.99 $ 点を失う．

ただし，ある座標において **モザイク化**することでスコアが上がる場合にはモザイク化を行ってスコアを計算する．**モザイク化**とは，２本の秘密配列を推定する際に途中で配列が入れ替わる推定ミスをしてしまった場合にそれを救済する操作である． **モザイク化**の例を以下に示す．復元した秘密文字列が以下の例では途中の１箇所（空白を入れて強調した．この空白の座標をモザイク座標と呼ぶ）で入れ替わってしまっているが，モザイク化を行うとモザイク座標前後で $ o_1,\ o_2 $ の配列を入れ替えることができ，以下の例ではモザイク化を行うことで $ o_1,\ o_2 $ に含まれている全ての文字が $ s_1,\ s_2 $ に一致している．ただし，モザイク化は最大で 1 回しか行うことができず，モザイク化を行うとペナルティとして$ 7.5 $点を失う．

#### モザイク化の例

 ```
s_1: GTC ACCGTGCAG
s_2: AACG ACGGACATG

o_1: AACG ACCGTGCAG
o_2: GTC ACGGACATG
```

### スコアに関する留意点１

本問題の入力データは完全に実データを用いて行っている．つまり，実際のヒトDNA配列をDNAシークエンサーに投入し，出力データの一部を切り取って用いている．また，正解となる２本の配列も実際のヒトDNA配列を DNAシークエンサーを含む様々な機器によって観測した桁違いに膨大なデータから業界でベストに近い知恵を集めて作成している．これは何を意味するかと言うと，入力データから満点となる２本の配列が出力できることは全く保証されていない．また，正解データとしてジャッジが用いているデータは極めて精度が高いと考えられるものの，100%正しいとは限らない．問題文に記述されていない偏りなども多く存在していると考えられる．判断に迷ったら，常にデータを信じて欲しい．

### スコアに関する留意点２

本問題では現実世界でより役に立つ解答をより髙い点数で評価したいと考えている．このため，現状でサーバーにアップロードされているデータセットのみに対して過学習したアルゴリズムの解答を低い点数で評価したい．例えば乱数シードを用いたアルゴリズムを作り，異なるシードの解答を多数アップロードして最も高い点数をたたき出した乱数シードを最終版とする，といった現実世界で役に立たない解答の点数を低くしたい．このため，プログラム提出が締め切られた後でジャッジデータを追加して最終採点とする．合計点の理論値最大は３万点を目指しているが，実データを元にしているため 10% 前後の誤差があることを予め承知されたい．

### サンプル1

２種類の短い秘密文字列があるパターンである．

### サンプル2

２種類の短い秘密文字列が完全に同一，もしくは違いがあっても入力からは違いを断定できないパターンである．

### もう少し大きなサンプル

ジャッジサーバの計算資源には限りがあり，提出は最大で２時間に１回に制限されている．参加者の皆様の手元の計算機上でデータを検討できるように，より実用的なサンプルデータをいくつかダウンロードできるように準備した．以下のデータはサンプルデータをゲノム業界の標準形式の一つである BAM ファイルに変換し，世界的に良く使われているビューワーの一つである [IGV](https://software.broadinstitute.org/software/igv/) で閲覧できる．IGV の利用方法については今後追記される．また，入力データと解答データを元に皆様の手元の計算機上で採点できるように[**採点プログラム**](https://github.com/exKAZUu/genocon2021-docker)を用意した．このプログラムを用いて手元の計算機で採点する場合には一切の制限がないため，デバッグや開発に役立てて欲しい．

以下の Answer Data には２行で秘密配列 $ s_1,\ s_2 $ に相当する配列が格納されている。但し、ジャッジが採点する際にスコアを高速に計算できるように $ s_1 $ と $ s_2 $ の正解ペアワイズアラインメントを作成し - を挿入することで長さを等しくしてある．実際に参加者が submit するべきプログラムはこのような - を挿入してはいけない．また、Answer Data には X という文字も含まれているが，これは採点に用いない配列領域を表している．本コンテストで用いたデータは本物のヒトDNA配列を用いているため，（参加者に提供したデータとは独立に取得した膨大な観測データからは）現在の科学レベルでは自信をもって確定できない DNA 配列が残っており，そのような領域を採点から外すためにマスクしてある．X に対応する領域は文字や文字の長さを間違えてもペナルティは課されない．

※本データセットは本コンテストに供するために Oxford Nanopore Technologies 社から提供されたデータを含んでいます．ここでダウンロードしたデータをコンテスト以外の目的に利用することはできません．また，コンテスト終了後にはデータは消去してください． **採点プログラム（gen1\_small\_10.testcase.txtを含む）と以下のデータのダウンロードには，IDとパスワードの入力が必要です．IDは「genocon2021」パスワードは「ontQ20」となります．IDとパスワードは他所にて開示することはしないでください．**

- gen1\_small10
  - [Input Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_10.testcase.txt)
  - [Answer Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_10.answer.txt)
  - [Sorted BAM](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_10.sorted.bam)
  - [Sorted BAM Index](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_10.sorted.bam.bai)
- gen1\_small12
  - [Input Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_12.testcase.txt)
  - [Answer Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_12.answer.txt)
  - [Sorted BAM](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_12.sorted.bam)
  - [Sorted BAM Index](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_12.sorted.bam.bai)
- gen1\_small13
  - [Input Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_13.testcase.txt)
  - [Answer Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_13.answer.txt)
  - [Sorted BAM](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_13.sorted.bam)
  - [Sorted BAM Index](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_13.sorted.bam.bai)
- gen1\_small14
  - [Input Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_14.testcase.txt)
  - [Answer Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_14.answer.txt)
  - [Sorted BAM](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_14.sorted.bam)
  - [Sorted BAM Index](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_14.sorted.bam.bai)
- gen1\_small15
  - [Input Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_15.testcase.txt)
  - [Answer Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_15.answer.txt)
  - [Sorted BAM](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_15.sorted.bam)
  - [Sorted BAM Index](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_15.sorted.bam.bai)
- gen1\_small17
  - [Input Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_17.testcase.txt)
  - [Answer Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_17.answer.txt)
  - [Sorted BAM](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_17.sorted.bam)
  - [Sorted BAM Index](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_17.sorted.bam.bai)
- gen1\_small18
  - [Input Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_18.testcase.txt)
  - [Answer Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_18.answer.txt)
  - [Sorted BAM](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_18.sorted.bam)
  - [Sorted BAM Index](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_18.sorted.bam.bai)
- gen1\_small19
  - [Input Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_19.testcase.txt)
  - [Answer Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_19.answer.txt)
  - [Sorted BAM](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_19.sorted.bam)
  - [Sorted BAM Index](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_19.sorted.bam.bai)
- gen1\_small20
  - [Input Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_20.testcase.txt)
  - [Answer Data](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_20.answer.txt)
  - [Sorted BAM](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_20.sorted.bam)
  - [Sorted BAM Index](https://iibmp2021.hamadalab.com/genocon/picked/gen1_small_20.sorted.bam.bai)

### 断り書き

本問題で提供するデータは Oxford Nanopore Technologies 社の開発している PromethION DNA シークエンサーと，一般にはまだ販売されていないQ20試薬を用いた同社提供の（公開許諾済みの）ヒトゲノムデータから作成していますが，今回提供されたデータは開発中の試薬を用いているため今後製品として同製品の一般販売が開始された場合の製品の性能を示すものではありません．

### 問題の背景

※ ***この項目は読まなくても問題を解くことができますが，出題の背景となりますため，ご興味を持ってくださった方はお読みいただけると幸いです．***

DNA の配列（A, C, G, T）を読み取る機械である DNA シークエンサーは染色体の端から端までを誤り無く読み取ることはできない．細胞からDNAを抽出する際に DNA が痛んでしまい，細かく千切れてしまうため，DNAシークエンサーのセンサー部分に全長の染色体をセットすることがそもそも不可能である．このため，現実世界では細かく千切れた DNA 断片の配列をたくさん読み取ってコンピューター処理により元々の DNA 配列を推定し復元する．読み取った DNA 配列は千切れているため，染色体のどの部分を読んだのかが分からず，染色体上のどこかランダムな位置から読まれた断片配列が読み取られる．

![](https://iibmp2021.hamadalab.com/genocon/prob_d_picture/overall.png)

読み取った断片配列が染色体上のどこから読まれた配列であるかは，ヒトの場合にはヒト参照ゲノムと呼ばれる標準的なヒトゲノム配列に対してペアワイズアラインメントを行うことで調べている．概ね９割ぐらいのヒトDNA配列はほとんど全ての人類で同じような順序で並んでいる．つまり，ヒト参照配列にマッチングを行うことで染色体のどの部分から出てきた断片配列であるかが分かる，ということである．残りの１割は標準的なヒト参照ゲノム配列に対してマッチングする場所が２箇所以上あり，染色体上のどこから得られた断片なのかが確定できなかったり，標準的な参照ヒトゲノム配列にはそもそも存在しない配列だったりする．

今回のコンテストで提供するデータは匿名の複数の人物から「世界中にデータを公開しても良い」という条件で頂いた DNA を実際に PromethION シークエンサーと最新のQ20試薬で読んだ断片配列を用いて作成している．コンテスト参加者に配っているサンプルデータからジャッジに用いるデータが類推できないように，コンテスト参加者に配ったデータとジャッジに用いるヒト DNA断片配列は異なる人物から得られた DNA 配列断片である．以下のスクリーンショットは IGV と呼ばれるゲノム断片配列ビューアーを用いて実際のデータを表示している例である．

![](https://iibmp2021.hamadalab.com/genocon/prob_d_picture/igv01.png)

観測試行の (1) において 50% の確率で方向を選んでいるのは DNA の２重螺旋のうちどちら側が DNA シークエンサーによって読まれるかを模しており，基本的に現実世界でも 50% の確率で２重螺旋のどちら側が選ばれるかが決まると思われている．ただし，実際にそれが成り立っているかどうかは誰も知らない．読み取った断片配列を参照ヒトゲノム配列にマッチングさせた際に方向を揃える処理を行うことが一般的であり，上記のスクリーンショットでは参照ヒトゲノム配列の方向に合わせて断片配列の向きを全て揃えてある．

観測試行の (2) では DNA 断片の長さを決めている．実際の分布はDNA断片を細胞から抽出する際の実験条件等に依存して複雑な形をしており，具体的な分布を事前に示すことは難しい．

DNAシークエンサーで読み取り可能な断片配列長は技術の進歩とともにどんどん長くなり，2000年頃には 1200 文字（1200塩基対）程度だった最大読み取り長は，PromethION ではほぼ無限と言われている．ただし，DNA 断片配列を壊さずにシークエンサーにセットできた世界最長の記録は 400万文字（400万塩基対）程度と言われている．何れにせよ，DNAは通常もっとずっと短く千切れてしまっているので連続した読み取り長は 1,000 文字から10万文字ぐらいとなるのが普通である．

DNAシークエンサーの読み取りは完璧では無く，観測エラーが発生する．このため，DNAシークエンサーにセットした DNA の配列とは若干異なる配列が読み取られて出力されることが多い．エラーがどのようなメカニズムで発生してどのような性質（分布）を持っているのかは科学的な興味の対象である．今回提供した PromethION の Q20+試薬を用いたデータは Oxford Nanopore Technologies が開発した最新の試薬を使っているため，エラーの性質（分布）については未知の部分も多い．簡単に言うと出題者にも確かなことは言えない，ということである．旧バージョンの試薬では多くの（$ 6 $文字以上）連続した AやTを読み取ろうとすると真の長さより短くなってしまう傾向があることが知られていた．今回の新試薬ではこのようなエラーが大きく減っていることが期待される．PromethION シークエンサーの小型版である MinION の動作原理について同社の[動画（英語）](https://www.youtube.com/watch?v=RcP85JHLmnI)がアニメーションで詳しく解説している．余裕があれば動画をぜひ見て欲しい．PromethION はポア（ＤＮＡを検知するセンサーの穴）の数が MinION より多いが，基本的な動作原理は同一である．

今回，参加者の皆様には参照ゲノム配列と PromethION の出力データの一部をお配りするので，新型試薬の観測エラー（シークエンシングエラー）の性質を推定し，２本の DNA 配列（ゲノム配列の一部）をなるべく正しく推定するプログラムを書いて欲しい．余談とはなるが，研究現場で最終的に達成したい精度は，エラーが 1,000,000 文字（塩基）につき 1塩基以下である．今回の問題で言えば全ての問題について満点に相当する．過去に行われた別のプログラミングコンテストでは，DNA 配列解析とは全く無縁のプログラマーが研究業界トップのプログラムを（コンテストで設定された基準で）超えるパフォーマンスをたたき出したと聞く．このコンテストでも業界トップの既知のアルゴリズムを超えるアルゴリズムが産まれたりはしないかと密かに期待をしているところである．Oxford Nanopore Technologies 社もおそらく同様の期待を抱いてのことだとは思うが， DNA 配列シークエンシングを行い本コンテストへのデータ提供を承諾してくれた．もしこの試みが上手く行けば PromethION を用いたゲノム解読が進歩して，がんの治療法やさまざまな遺伝病の原因発見が大きく加速するかも？

### Sample Explanation 1

\#### 入力をマルチプルアラインメント形式に見やすく表示したもの Gは参照配列を表す． ``` G : ACACAGCGGCGACC 0 &gt;: ACATAGCGGCGACC 1 &lt;: ACACAGCGGCGACC 2 &lt;: ACACAGCGG-GACC 3 &lt;: ACACAGCGGCGACC 4 &lt;: ACACAGCGGCGACC 5 &lt;: ACACAGCGG-GACC ```

### Sample Explanation 2

\#### 入力をマルチプルアラインメント形式に見やすく表示したもの ``` R : ACCGGTTG-GCGTG 0 &gt;: ACCGG 1 &lt;: CCGGTTG-G 2 &gt;: CGATTGCGCG 3 &lt;: GTTG-G-GT 4 &gt;: G-GCGTG ```