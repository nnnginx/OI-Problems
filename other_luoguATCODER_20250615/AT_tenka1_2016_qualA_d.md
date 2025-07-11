# AT_tenka1_2016_qualA_d グラフィカルグラフ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tenka1-2016-quala/tasks/tenka1_2016_qualA_d

*天下一株式会社では、グラフ理論におけるグラフを視覚的に表現するソフトウェアを開発しています。 特に、あまり複雑でないグラフをテキストベースで見やすく表示するツールが人気です。*

$ N $ 頂点の無向木が与えられます。 各頂点には、大文字のアルファベットが重複なく割り振られています（頂点の個数は $ 26 $ 以下です）。

$ N-1 $ 本の辺のうち $ i $ 番目は、頂点 $ v_i $ と頂点 $ w_i $ を結びます。 ただし、任意の頂点について、その頂点に接続する辺の本数が $ 4 $ 以下であることが保証されます。

与えられた木を以下のように視覚的に表示するプログラムを作ってください。 詳細は「出力」セクションに記します。

 ```
8 12
............
...D...E....
...|...|....
.C-A---B---F
.|.....|...|
.|.....G.J-I
.H..........
............
```

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ v_1 $ $ w_1 $ $ v_2 $ $ w_2 $ $ : $ $ v_{N-1} $ $ w_{N-1} $

## 输出格式

入力された木を、以下の形式で $ H+1 $ 行に表示せよ。

> $ H $ $ W $ $ c_{1,1} $$ c_{1,2} $ $ … $ $ c_{1,W} $ $ c_{2,1} $$ c_{2,2} $ $ … $ $ c_{2,W} $ $ : $ $ c_{H,1} $$ c_{H,2} $ $ … $ $ c_{H,W} $

ここで、

- $ H $, $ W $ は以下に続く視覚表示の大きさを表し、半角スペース一つで区切られる。$ 1≦H≦100,\ 1≦W≦100 $ を満たさなければならない。
- 視覚表示は、文字を縦 $ H $ 文字、横 $ W $ 文字の長方形状に並べたものである。
- 視覚表示を構成するそれぞれの文字 $ c_{i,j} $ は、英大文字の最初の $ N $ 文字および `.`、`-`、`|` のいずれかであり、以下を満たす。
  - 木の各頂点は、対応する英大文字で表される。それぞれの頂点は、視覚表示にちょうど一度ずつ現れなければならない。
  - 頂点を表す文字は、別の頂点を表す文字と縦または横に隣接してはならない。
  - 二つの頂点 $ a,\ b $ が一本の辺で直接結ばれるなら、以下の条件 **(A)**, **(B)** のうち一方を満たさなければならない。
      - **(A)** 頂点 $ a,\ b $ を表す二つの文字が視覚表示の同じ行にあり、それらに挟まれた文字はすべて `-` である。
      - **(B)** 頂点 $ a,\ b $ を表す二つの文字が視覚表示の同じ列にあり、それらに挟まれた文字はすべて `|` である。
  - 二つの頂点 $ a,\ b $ が一本の辺で直接結ばれないなら、上記の条件 **(A)**, **(B)** を満たすことはどちらも禁止される。
  - 以上のように頂点や辺を表す文字以外の文字は、すべて `.` でなければならない。

なお、制約を満たす入力に対し、これらの条件を満たす視覚表示が必ず存在することが示せる。そのような視覚表示のうち、どれを出力してもよい。

## 输入输出样例 #1

### 输入 #1

```
10
A B
A C
A D
B E
B F
B G
C H
F I
I J
```

### 输出 #1

```
8 12
............
...D...E....
...|...|....
.C-A---B---F
.|.....|...|
.|.....G.J-I
.H..........
............
```

## 输入输出样例 #2

### 输入 #2

```
7
A B
B C
C D
D E
E F
F G
```

### 输出 #2

```
5 4
.A-B
E-F|
|.||
|.G|
D--C
```

## 说明/提示

### 制約

- $ 2≦N≦26 $
- $ v_i $, $ w_i $ は、それぞれ英大文字の最初の $ N $ 文字のいずれかである。
- 与えられるグラフは木である。
- 任意の頂点について、その頂点に接続する辺の本数は $ 4 $ 以下である。

### Sample Explanation 1

出力例は問題文中で示した例と同一です。

### Sample Explanation 2

頂点を表す文字が `-` や `|` と縦や横に隣接することは禁止されていません。