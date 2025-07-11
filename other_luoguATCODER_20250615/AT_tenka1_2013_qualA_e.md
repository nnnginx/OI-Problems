# AT_tenka1_2013_qualA_e 天下一ジグソーパズル

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tenka1-2013-quala/tasks/tenka1_2013_qualA_e

 天下一プログラマーコンテストのモノクロポスターが、高橋君のいたずらにより、バラバラにされてしまいました。  
 ポスターは、H\*W個の正方形のタイルを、縦H個、横W個の長方形に敷き詰めて構成されていたのですが、高橋君によって、全てタイル４つで構成される、トの字型のピースに分解されてしまっています。  
 幸運なことに、元のデジタルデータは残っていましたが、残念なことに、印刷するための紙がありません。  
 仕方がないので、あなたはこのピースから、ポスターを修復しなければいけません。

 入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ S_1 $ $ S_2 $ : : $ S_H $ $ N $ $ P_1 $ $ P_2 $ : : $ P_n $

- $ 1 $ 行目には、ポスターの縦の長さ $ H $ と横の長さ$ W $($ 4\ \leq\ H,W\ \leq\ 12 $)が、スペースで区切られて、それぞれ整数で与えられる。
- $ H,\ W $はそれぞれ$ 4 $で必ず割り切れる。

- $ 2 $ 行目から$ H $行は、元のポスターを表す文字列 $ S_i $ が与えられる。この文字列は各行とも $ W $文字である。
- $ S_i $の$ j $文字目は、左上のタイルを$ (1,1) $とした座標$ (j,i) $における、タイルの色を表す。 '#'が黒いタイル、'.'が白いタイルを表す。

- $ H\ +\ 2 $行目には、ピースの数$ N $が与えられる。
- $ H\ +\ 3 $行目から$ N $($ N\ =\ H\ *\ W\ /\ 4 $)行には、与えられるピースの模様の種類$ P_i $($ 1\ \leq\ P_i\ \leq\ 16 $)が与えられる。模様の種類は以下の16種類である。
 
```
<pre class="prettyprint linenums">
.   #   .   #   .   #   .   #   .   #   .   #   .   #   .   #  
..  ..  #.  #.  .#  .#  ##  ##  ..  ..  #.  #.  .#  .#  ##  ## 
.   .   .   .   .   .   .   .   #   #   #   #   #   #   #   #  
1   2   3   4   5   6   7   8   9   10  11  12  13  14  15  16
```

- $ H,\ W\ \leq\ 4 $ の入力に正解すると、$ 150 $ 点満点に対して部分点として $ 30 $ 点が与えられる
- $ H,\ W\ \leq\ 8 $ の入力に正解すると、$ 150 $ 点満点に対して部分点として追加で $ 50 $ 点が与えられる

 パズルを修復する方法を $ n $ 行で出力してください。パズルが復元不可能である場合は、-1と出力してください。  
 i行目には、$ P_i $の置くべき$ X $座標、$ Y $座標、回転方向の3つの整数をスペース区切りで出力してください。 なお、回転方向は、下図のように時計回りに表し、ポスターの左上の座標を$ (1,\ 1) $とし、下記の図のAの位置の座標を出力するとします。

```
<pre class="prettyprint linenums">
A  DBA    D     
BC  C    CB  C  
D         A ABD 
0  1    2   3
```

 なお、行の終端には改行が必要です。答えが複数ある場合は、どれを出力しても構いません。 ```

4 4
#...
.#..
..##
..##
4
9
6
1
8
```

 ```

1 4 3
1 1 0
4 1 1
4 4 2
```

- 下記の図のように、元のポスターを修復することが可能である。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_tenka1_2013_qualA_e/9679bde5561ce2148ffc33728f9e8c1ceab2f0b5.png)図 $ 1 $：復元したポスター

 

 ```

4 4
#...
.#..
..##
..##
4
1
2
3
4
```

 ```

-1
```

- 与えられたピースから元のポスターがどうやっても復元できない場合は、-1を出力する。

## 输入格式

无

## 输出格式

无