## 题目描述
[problemUrl]: https://atcoder.jp/contests/dp/tasks/dp_h

縦 $ H $ 行、横 $ W $ 列のグリッドがあります。 上から $ i $ 行目、左から $ j $ 列目のマスを $ (i,\ j) $ で表します。

各 $ i,\ j $ ($ 1\ \leq\ i\ \leq\ H $, $ 1\ \leq\ j\ \leq\ W $) について、マス $ (i,\ j) $ の情報が文字 $ a_{i,\ j} $ によって与えられます。 $ a_{i,\ j} $ が `.` ならばマス $ (i,\ j) $ は空マスであり、$ a_{i,\ j} $ が `#` ならばマス $ (i,\ j) $ は壁のマスです。 マス $ (1,\ 1) $ および $ (H,\ W) $ は空マスであることが保証されています。

太郎君は、マス $ (1,\ 1) $ から出発し、右または下に隣り合う空マスへの移動を繰り返すことで、マス $ (H,\ W) $ まで辿り着こうとしています。

マス $ (1,\ 1) $ から $ (H,\ W) $ までの太郎君の経路は何通りでしょうか？ 答えは非常に大きくなりうるので、$ 10^9\ +\ 7 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ a_{1,\ 1} $$ \ldots $$ a_{1,\ W} $ $ : $ $ a_{H,\ 1} $$ \ldots $$ a_{H,\ W} $

## 输出格式
マス $ (1,\ 1) $ から $ (H,\ W) $ までの太郎君の経路は何通りか？ $ 10^9\ +\ 7 $ で割った余りを出力せよ。

## 题目大意
给一个 $H\times W$ 的网格，一开始在左上角 $(1,1)$ 每一步只能向右或向下走，不能经过 '#' 格子，求走到右下角 $(H,W) $ 有多少种走法。  

答案对 $10^9+7$ 取模。

```input1
3 4
...#
.#..
....
```

```output1
3
```

```input2
5 2
..
#.
..
.#
..
```

```output2
0
```

```input3
5 5
..#..
.....
#...#
.....
..#..
```

```output3
24
```

```input4
20 20
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
....................
```

```output4
345263555
```

## 提示
### 制約

- $ H $ および $ W $ は整数である。
- $ 2\ \leq\ H,\ W\ \leq\ 1000 $
- $ a_{i,\ j} $ は `.` または `#` である。
- マス $ (1,\ 1) $ および $ (H,\ W) $ は空マスである。

### Sample Explanation 1

経路は次図の $ 3 $ 通りです。 !\[\](https://img.atcoder.jp/dp/grid\_0\_0\_muffet.png)

### Sample Explanation 2

経路が存在しない場合もあります。

### Sample Explanation 4

答えを $ 10^9\ +\ 7 $ で割った余りを出力することを忘れずに。

