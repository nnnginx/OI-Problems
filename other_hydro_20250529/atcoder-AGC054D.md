## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc054/tasks/agc054_d

`(`, `)`, `o`, `x` からなる文字列 $ S $ が与えられます． あなたは，$ S $ の隣接する $ 2 $ 文字をswapする操作を好きな回数行うことができます． 次の条件を達成するために必要な最小の操作回数を求めてください．

- $ S $ に登場するすべての `o` を `()` で，`x` を `)(` で置き換え，`(` と `)` のみからなる文字列 $ S' $ を作る． この時，$ S' $ は**括弧の対応が取れている文字列**である．
 
括弧の対応が取れている文字列の定義 括弧の対応が取れている文字列とは，次のうちいずれかの条件を満たす文字列です．

- 空文字列
- ある括弧の対応が取れている空でない文字列 $ s,\ t $ が存在し，$ s,\ t $ をこの順に連結した文字列
- ある括弧の対応が取れている文字列 $ s $ が存在し、 `(`, $ s $, `)` をこの順に連結した文字列

なお，この問題の制約より，目標を達成することは必ず可能です．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ S $

## 输出格式
答えを出力せよ．

## 题目大意
给定一个串 $S$ 包含 `(`, `)`, `o`, `x`。

求最小的交换次数使得交换后的串将 `o` 替换为 `()`， `x` 替换为 `)(` 后，是一个合法括号序列。

```input1
)x(
```

```output1
3
```

```input2
()ox
```

```output2
2
```

```input3
()oxo(xxx))))oox((oooxxoxo)oxo)ooo(xxx(oox(x)(x()x
```

```output3
68
```

## 提示
### 制約

- $ S $ は `(`, `)`, `o`, `x` からなる文字列
- $ S $ は $ 1 $ つ以上の `(` と `)` を含み，またそれらの個数は等しい
- $ |S|\ \leq\ 8000 $

### Sample Explanation 1

`)x(` → `x)(` → `x()` → `(x)` と操作すればよいです． このとき，$ S'= $`()()` であり，これは括弧の対応の取れている文字列です．

