# AT_wupc2012_4 三角パズル

## 题目描述

[problemUrl]: https://atcoder.jp/contests/wupc2012/tasks/wupc2012_4

 そうこうしているうちに，圧縮ファイルの解凍が終わったようだ．中を見ると，今度は直角三角形状に並んだ数列を含むテキストファイルを見つけた．  
  
 7  
 2 3  
 1 5 4  
  
 どうやら，一番上の頂点からはじめて，一段下の直下か右下かを選び底辺まで下っていったとき，その経路中の数値の合計の最大値を求める問題のようだ．それなら簡単．上の例の場合，7 -&gt; 3 -&gt; 5 と選ぶのが最適で，合計は 15 となる．しかし，このようなファイルはたくさんあり，中には100段に及ぶデータもあった．これを解かなきゃ参加資格はないってことか…？  
 いやまて，これはプログラミングコンテストへの招待状だ．数列を入力として与えた時，最大値を求めるプログラムを作ってしまえばいい．おそらく，招待状を送った人物はそれを期待している．  
 以下のように直角三角形上に並んだ数列が与えられる．頂点から初めて一段下の直下か右下を選び，底辺まで下ったときの経路中の数値の合計の最大値を求めよ．  
 例えば，以下のような数列が与えられたとすると，  
  
 3  
 7 4  
 2 4 6  
 8 5 9 3  
  
 正しく選択した場合，  
  
**3**  
**7** 4  
 2 **4** 6  
 8 5 **9** 3  
  
 であり，合計値は 3 + 7 + 4 + 9 = 23 となる． 入力は以下の形式で標準入力から与えられる．

> $ N $ $ a_{1,1} $ $ a_{2,1}　a_{2,2} $ $ a_{3,1}　a_{3,2}　a_{3,3} $ $ ... $ $ a_{i,1}　a_{i,2}　...　a_{i,i} $ $ ... $ $ a_{N,1}　a_{N,2}　...　a_{N,N} $

- $ 1 $ 行目には直角三角形の高さ $ N $($ 1\ ≦\ N\ ≦\ 100 $) が与えられる．
- $ i $ 行目($ 2\ ≦\ i\ ≦\ N+1 $)には数字が半角スペース区切りで $ i-1 $ 個与えられる．
- 数列に含まれる数は $ 0\ ≦\ a_{i,j}\ ≦\ 100 $($ 1\ ≦\ j\ ≦\ i\ ≦\ N $) を満たす．
 
 数値の合計の最大値を標準出力に $ 1 $ 行で出力せよ．  
 100点満点中，50点分については，$ N\ ≦\ 20 $ を満たす．

## 输入格式

无

## 输出格式

无