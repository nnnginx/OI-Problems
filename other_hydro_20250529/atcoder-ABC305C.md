## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc305/tasks/abc305_c

縦 $ H $ マス, 横 $ W $ マスのグリッドがあります。上から $ i $ 行目、左から $ j $ 列目のマスを $ (i,\ j) $ と呼びます。  
 はじめ、グリッド上には、ある **縦横 $ 2 $ マス以上** の部分長方形の内部にあるマスにクッキーが 1 枚ずつ置かれていて、それ以外のマスにはクッキーが置かれていません。  
 形式的に説明すると、以下の条件を全て満たす 4 つの整数の組 $ (a,b,c,d) $ がただ 1 つ存在します。

- $ 1\ \leq\ a\ \lt\ b\ \leq\ H $
- $ 1\ \leq\ c\ \lt\ d\ \leq\ W $
- グリッド上のマスのうち、$ a\ \leq\ i\ \leq\ b,\ c\ \leq\ j\ \leq\ d $ を満たす全てのマス $ (i,\ j) $ にはクッキーが 1 枚ずつ置かれていて、それ以外のマスにはクッキーが置かれていない。
 
ところが、すぬけ君がグリッド上のクッキーのどれか 1 枚を取って食べてしまいました。  
 すぬけ君がクッキーを取ったマスは、クッキーが置かれていない状態に変わります。

すぬけ君がクッキーを食べた後のグリッドの状態が入力として与えられます。  
 マス $ (i,\ j) $ の状態は文字 $ S_{i,j} $ として与えられて、`#` はクッキーが置かれているマスを, `.` はクッキーが置かれていないマスを意味します。  
 すぬけ君が食べたクッキーが元々置かれていたマスを答えてください。(答えは一意に定まります。)

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ S_{1,1} $$ S_{1,2} $$ \dots $$ S_{1,W} $ $ S_{2,1} $$ S_{2,2} $$ \dots $$ S_{2,W} $ $ \vdots $ $ S_{H,1} $$ S_{H,2} $$ \dots $$ S_{H,W} $

## 输出格式
すぬけ君が食べたクッキーが元々置かれていたマスを $ (i,\ j) $ とする。$ i,\ j $ をこの順に空白区切りで出力せよ。

## 题目大意
有一个 $H$ 行 $W$ 列的网格图。

网格图上存在一个唯一的矩阵，其边长都不小于 $2$，这个矩阵中的每个网格上都有一块曲奇（记为 `#`），而这个矩阵之外的所有格子上都没有曲奇（记为 `.`）。

现在，Snuke 吃掉了其中的一块曲奇，给出吃掉曲奇以后的网格图状态，你需要给出被吃掉的曲奇的位置。行坐标从上到下计算，列坐标从左到右计算，坐标从 $1$ 开始。

- $2\leq H,W\leq500$
- 网格图中的每个字符都是 `#` 或 `.`

```input1
5 6
......
..#.#.
..###.
..###.
......
```

```output1
2 4
```

```input2
3 2
#.
##
##
```

```output2
1 2
```

```input3
6 6
..####
..##.#
..####
..####
..####
......
```

```output3
2 5
```

## 提示
### 制約

- $ 2\ \leq\ H,\ W\ \leq\ 500 $
- $ S_{i,j} $ は `#` または `.`
 
### Sample Explanation 1

はじめ、クッキーは $ (2,\ 3) $ を左上、$ (4,\ 5) $ を右下とする部分長方形の内部にあるマスに置かれていて、すぬけ君は $ (2,\ 4) $ にあるクッキーを食べたことがわかります。よって $ (2,\ 4) $ を出力します。

### Sample Explanation 2

はじめ、クッキーは $ (1,\ 1) $ を左上、$ (3,\ 2) $ を右下とする部分長方形の内部にあるマスに置かれていて、すぬけ君は $ (1,\ 2) $ にあるクッキーを食べたことがわかります。

