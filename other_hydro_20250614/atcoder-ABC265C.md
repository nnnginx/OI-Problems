## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc265/tasks/abc265_c

縦 $ H $ マス、横 $ W $ マスのグリッドがあります。上から $ i $ 行目、左から $ j $ 列目のマスを $ (i,j) $ と表します。  
 $ (i,j) $ には文字 $ G_{i,j} $ が書きこまれています。ここで $ G_{i,j} $ は `U`, `D`, `L`, `R` のいずれかです。

あなたは $ (1,1) $ にいます。あなたは移動することができなくなるまで次の操作を繰り返します。

> あなたは現在 $ (i,j) $ にいるとする。  
>  $ G_{i,j} $ が `U` であり、かつ $ i\ \neq\ 1 $ ならば $ (i-1,j) $ へ移動する。  
>  $ G_{i,j} $ が `D` であり、かつ $ i\ \neq\ H $ ならば $ (i+1,j) $ へ移動する。  
>  $ G_{i,j} $ が `L` であり、かつ $ j\ \neq\ 1 $ ならば $ (i,j-1) $ へ移動する。  
>  $ G_{i,j} $ が `R` であり、かつ $ j\ \neq\ W $ ならば $ (i,j+1) $ へ移動する。  
>  それ以外の場合、あなたは移動することができない。

操作を終了した時点であなたがいるマスを出力してください。  
 ただし、あなたが操作を終了することなく無限に移動し続ける場合は `-1` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ G_{1,1}G_{1,2}\dots\ G_{1,W} $ $ G_{2,1}G_{2,2}\dots\ G_{2,W} $ $ \vdots $ $ G_{H,1}G_{H,2}\dots\ G_{H,W} $

## 输出格式
操作を終了した時点であなたが $ (i,j) $ にいる場合は次の形式で出力せよ。

> $ i $ $ j $

また、無限に動き続ける場合は `-1` を出力せよ。

## 题目大意
给定一个矩阵 $g$，里面有许许多多的 `LRUD` 四个字母。

一个机器人从点 $(1,1)$ 出发，假设它到了点 $(x,y)$，则：

如果 $g_{x,y}$ 是 `U`，移动到 $(x-1,y)$。

如果 $g_{x,y}$ 是 `D`，移动到 $(x+1,y)$。

如果 $g_{x,y}$ 是 `L`，移动到 $(x,y-1)$。

如果 $g_{x,y}$ 是 `R`，移动到 $(x,y+1)$。

如果某一次移动后，小机器人走出了这个矩阵，输出在哪里走出的方格。如果小机器人不可能走出矩阵就输出 $-1$。

```input1
2 3
RDU
LRU
```

```output1
1 3
```

```input2
2 3
RRD
ULL
```

```output2
-1
```

```input3
9 44
RRDDDDRRRDDDRRRRRRDDDRDDDDRDDRDDDDDDRRDRRRRR
RRRDLRDRDLLLLRDRRLLLDDRDLLLRDDDLLLDRRLLLLLDD
DRDLRLDRDLRDRLDRLRDDLDDLRDRLDRLDDRLRRLRRRDRR
DDLRRDLDDLDDRLDDLDRDDRDDDDRLRRLRDDRRRLDRDRDD
RDLRRDLRDLLLLRRDLRDRRDRRRDLRDDLLLLDDDLLLLRDR
RDLLLLLRDLRDRLDDLDDRDRRDRLDRRRLDDDLDDDRDDLDR
RDLRRDLDDLRDRLRDLDDDLDDRLDRDRDLDRDLDDLRRDLRR
RDLDRRLDRLLLLDRDRLLLRDDLLLLLRDRLLLRRRRLLLDDR
RRRRDRDDRRRDDRDDDRRRDRDRDRDRRRRRRDDDRDDDDRRR
```

```output3
9 5
```

## 提示
### 制約

- $ 1\ \leq\ H,\ W\ \leq\ 500 $
- $ G_{i,j} $ は `U`, `D`, `L`, `R` のいずれかである。
- $ H,\ W $ は整数である。

### Sample Explanation 1

あなたは $ (1,\ 1)\ \to\ (1,\ 2)\ \to\ (2,\ 2)\ \to\ (2,\ 3)\ \to\ (1,\ 3) $ の順に動いたあとに操作を終了します。よって答えは $ (1,\ 3) $ です。

### Sample Explanation 2

あなたは $ (1,\ 1)\ \to\ (1,\ 2)\ \to\ (1,\ 3)\ \to\ (2,\ 3)\ \to\ (2,\ 2)\ \to\ (2,\ 1)\ \to\ (1,\ 1)\ \to\ (1,\ 2)\ \to\ \dots $ というように無限に動き続けます。この場合は `-1` を出力します。

