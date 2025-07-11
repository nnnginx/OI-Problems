# AT_arc012_3 [ARC012C] 五目並べチェッカー

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc012/tasks/arc012_3

高橋君は、五目並べが大好きです。  
 五目並べとは、 $ 19 $ × $ 19 $ の碁盤の上に交互に碁石を $ 1 $ つずつ並べ、 $ 5 $ つ以上の碁石が縦・横・ななめに並べたプレーヤーが勝ちとなってゲームが終了する、というルールのゲームです。  
 ゲームは必ず黒のプレーヤーから始めるものとします。  
 高橋君は、友達の青木君と五目並べをしていたのですが、うっかり居眠りをしてしまいました。  
 高橋君は寝ている間に青木君が不正をしたのではないかと疑っているので、盤面から五目並べの状態として異常なところがないかを探したいです。  
 五目並べの状態として、正常であるかどうか判定するプログラムを作ってください。  
 ここでの異常な状態とは、

- どちらかのプレーヤーの勝利条件を満たしているのに、もう片方のプレーヤーがさらに碁石を置いている。
- お互いが置いた個数がありえない状態になっている。
 
 のどちらかであることを指します。 入力は以下の形式で標準入力から与えられる。 > $ b_{1,1}\ b_{2,1}\ ‥‥\ b_{19,1} $ $ b_{1,2}\ b_{2,2}\ ‥‥\ b_{19,2} $ $ : $ $ : $ $ b_{1,19}\ b_{2,19}\ ‥‥\ b_{19,19} $

- 入力は $ 19 $ 行与えられる。
- $ i(1≦i≦19) $ 行目の $ j(1≦j≦19) $ 文字目には、盤面の縦 $ i $ 番目、横 $ j $ 番目のマスの情報を表す文字 $ b_{i,j} $ が与えられる。
- $ b_{i,j} $ は、`o`、`x`、`.` の $ 3 $ 種類のいずれかの文字である。 
  - `o` は、黒石が置かれていることを表す。
  - `x` は、白石が置かれていることを表す。
  - `.` は、何も置かれていないことを表す。


 盤面が正常な状態であれば、`YES`、そうでなければ `NO` と出力しなさい。   
 出力は標準出力におこない、末尾には改行をいれること。  
```

...................
...................
...................
...................
....x......o.......
...................
...................
.......o....o......
...................
........x..........
..............o....
...................
.......x...........
...................
...................
...................
...................
...................
...................
```

 ```

YES
```

- 黒が $ 4 $ 手、白が $ 3 $ 手打った状態です。
- （記述に誤りがありましたので、修正しました。）
 
```

...................
...................
...................
...................
....x......o.......
...................
...................
.......o....o......
...................
........x..........
..............o....
...................
.......x...........
...................
...................
.........o.........
...................
...................
...................
```

 ```

NO
```

- 黒が $ 5 $ 手、白が $ 3 $ 手打った状態です。
- 黒が $ 1 $ 手多く打ってしまっているので、異常な状態です。
 
```

...................
...................
...................
...................
...................
...................
...................
...................
........ooooo......
.........xxxx......
........x..........
...................
...................
...................
...................
...................
...................
...................
...................
```

 ```

NO
```

- 黒が $ 5 $ 手、白が $ 5 $ 手打った状態です。
- 片方が勝利条件を満たしていればゲームは終了しているので、黒が勝利条件を満たしているのは異常な状態です。
- （記述に間違いがありましたので、訂正しました。）
 
```

...................
...................
...................
...................
...................
...................
...................
...................
........ooooo......
.........xxxx......
...................
...................
...................
...................
...................
...................
...................
...................
...................
```

 ```

YES
```

- 黒が $ 5 $ 手、白が $ 4 $ 手打った状態です。
- 黒が $ 5 $ つ並べて勝利した状態となり、正常です。
 
```

...................
...................
...................
...................
...................
...................
...................
...................
.........x.........
......oooooo.......
........xxxx.......
...................
...................
...................
...................
...................
...................
...................
...................
```

 ```

YES
```

- 黒石が $ 6 $ つ並んでいますが、正常です。
- 例えば黒石が $ 2 $ つ並んでおり、$ 1 $ マス空いてさらに $ 3 $ つ並んでいる状態で、空いている真ん中のマスに黒石を置いた場合このような形になります。
 
```

...................
...................
...................
...................
...................
...................
........x..........
........x....x.....
...........x.......
...oooooooooo......
...................
......x......x.....
....x......x.......
.........x.........
...................
...................
...................
...................
...................
```

 ```

NO
```

- 黒が $ 10 $ 手、白が $ 9 $ 手打った状態です。
- 黒石を $ 10 $ 個並べる前に、黒が勝利してゲームが終了していないとおかしいので、異常な状態です。
 
```

...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
...................
```

 ```

YES
```

- 黒が高橋君で、一手も打たないうちに居眠りしてしまった場合も、正常な状態です。

## 输入格式

无

## 输出格式

无