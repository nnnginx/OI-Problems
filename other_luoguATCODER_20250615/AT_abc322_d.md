# AT_abc322_d [ABC322D] Polyomino

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc322/tasks/abc322_d

いくつかの正方形を辺でつなげてできる、連結な多角形の形をしたパズルのピースのことを **ポリオミノ** と呼びます。

縦 $ 4 $ マス、横 $ 4 $ マスのグリッドと、グリッドに収まる大きさの $ 3 $ 個のポリオミノがあります。  
 $ i $ 番目のポリオミノの形は $ 16 $ 個の文字 $ P_{i,j,k} $ ($ 1\ \leq\ j,\ k\ \leq\ 4 $) によって表されます。$ P_{i,\ j,\ k} $ は何も置かれていないグリッドに $ i $ 番目のポリオミノを置いたときの状態を意味して、$ P_{i,\ j,\ k} $ が `#` の場合は上から $ j $ 行目、左から $ k $ 列目のマスにポリオミノが置かれていることを、`.` の場合は置かれていないことを意味します。(入出力例 $ 1 $ の図も参考にしてください。)

あなたは次の条件を全て満たすように $ 3 $ 個のポリオミノ全てをグリッドに敷き詰めることにしました。

- グリッドの全てのマスはポリオミノで覆われている。
- ポリオミノ同士が重なるように置くことはできない。
- ポリオミノがグリッドからはみ出るように置くことはできない。
- ポリオミノの平行移動と回転は自由に行うことができるが、裏返すことはできない。
 
条件を満たすようにグリッドにポリオミノを敷き詰めることは可能ですか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ P_{1,1,1}P_{1,1,2}P_{1,1,3}P_{1,1,4} $ $ P_{1,2,1}P_{1,2,2}P_{1,2,3}P_{1,2,4} $ $ P_{1,3,1}P_{1,3,2}P_{1,3,3}P_{1,3,4} $ $ P_{1,4,1}P_{1,4,2}P_{1,4,3}P_{1,4,4} $ $ P_{2,1,1}P_{2,1,2}P_{2,1,3}P_{2,1,4} $ $ P_{2,2,1}P_{2,2,2}P_{2,2,3}P_{2,2,4} $ $ P_{2,3,1}P_{2,3,2}P_{2,3,3}P_{2,3,4} $ $ P_{2,4,1}P_{2,4,2}P_{2,4,3}P_{2,4,4} $ $ P_{3,1,1}P_{3,1,2}P_{3,1,3}P_{3,1,4} $ $ P_{3,2,1}P_{3,2,2}P_{3,2,3}P_{3,2,4} $ $ P_{3,3,1}P_{3,3,2}P_{3,3,3}P_{3,3,4} $ $ P_{3,4,1}P_{3,4,2}P_{3,4,3}P_{3,4,4} $

## 输出格式

問題文の条件を満たすようにポリオミノを敷き詰めることが可能である場合は `Yes` を、そうでない場合は `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
....
###.
.#..
....
....
.###
.##.
....
..#.
.##.
.##.
.##.
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
###.
#.#.
##..
....
....
..#.
....
....
####
##..
#...
#...
```

### 输出 #2

```
Yes
```

## 输入输出样例 #3

### 输入 #3

```
##..
#..#
####
....
....
##..
.##.
....
.#..
.#..
.#..
.#..
```

### 输出 #3

```
No
```

## 输入输出样例 #4

### 输入 #4

```
....
..#.
....
....
....
..#.
....
....
....
..#.
....
....
```

### 输出 #4

```
No
```

## 输入输出样例 #5

### 输入 #5

```
....
####
#...
#...
....
####
...#
..##
....
..##
..#.
..##
```

### 输出 #5

```
No
```

## 输入输出样例 #6

### 输入 #6

```
###.
.##.
..#.
.###
....
...#
..##
...#
....
#...
#...
#...
```

### 输出 #6

```
Yes
```

## 说明/提示

### 制約

- $ P_{i,\ j,\ k} $ は `#` または `.`
- 与えられるポリオミノは連結である。つまり、ポリオミノを構成する正方形同士は、正方形のみを上下左右に辿って互いに行き来できる
- 与えられるポリオミノは空でない
 
### Sample Explanation 1

入力例 $ 1 $ に対応するポリオミノの形は次の図のようになります。 !\[image1\](https://img.atcoder.jp/abc322/f0e25c2abcdbeade76fcb12eaee39f23.jpg) この場合、次の図のようにポリオミノを配置することで、問題文の条件を満たすようにグリッドにポリオミノを敷き詰めることができます。 !\[image2\](https://img.atcoder.jp/abc322/81e983f85e958e0d612063adcc455c71.jpg) よって答えは `Yes` になります。

### Sample Explanation 2

入力例 $ 2 $ の $ 1 $ 番目のポリオミノのように、ポリオミノは穴の空いた多角形の形をしている場合があります。

### Sample Explanation 3

ポリオミノを敷き詰めるときに、ポリオミノを裏返してはならないのに注意してください。