# AT_abc088_d [ABC088D] Grid Repainting

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc088/tasks/abc088_d

縦 $ H $ マス, 横 $ W $ マスに広がるマス目があり, 各マスは白または黒で塗られている. 上から $ i $ 番目で左から $ j $ 番目のマスを $ (i,\ j) $ で表す. すぬけ君は, このマス目を使って次のようなゲームをしたい. ゲームの開始時点ではマス $ (1,\ 1) $ にゲームキャラクター「けぬす君」がいる. プレイヤーはけぬす君を上下左右の $ 4 $ 方向のいずれかに $ 1 $ マスだけ動かすことを繰り返す. けぬす君が白いマスだけを通って $ (H,\ W) $ にたどり着けばゲームクリアとなる.  
 ゲームを開始する前に, すぬけ君はいくつかの白いマス目の色を黒に変えることができる. ただし, マス $ (1,\ 1) $ と $ (H,\ W) $ の色を変えることはできず, ゲームを開始するまでにすべての色の変更を行わなければならない.  
 ゲームをクリアしたとき, ゲームの開始前にマスの色を変えた回数がすぬけ君のスコアとなる. そのとき, すぬけ君が取る可能性のある最大のスコアを求めなさい.ただし, すぬけ君がどのようにマス目の色を変えてもけぬす君が $ (H,\ W) $ にたどり着くことが出来ない場合、$ -1 $ と出力しなさい.

ただし, 各マスの色の情報は文字 $ s_{i,\ j} $ として与えられる. マス $ (i,\ j) $ が最初白で塗られている場合 $ s_{i,\ j} $ は `.` であり, マス $ (i,\ j) $ が最初黒で塗られている場合 $ s_{i,\ j} $ は `#` である.

## 输入格式

入力は以下の形式で標準入力から与えられる.

> $ H $ $ W $ $ s_{1,\ 1}s_{1,\ 2}s_{1,\ 3}\ ...\ s_{1,\ W} $ $ s_{2,\ 1}s_{2,\ 2}s_{2,\ 3}\ ...\ s_{2,\ W} $ $ : $ $ : $ $ s_{H,\ 1}s_{H,\ 2}s_{H,\ 3}\ ...\ s_{H,\ W} $

## 输出格式

すぬけ君が取る可能性のある最大のスコアを出力しなさい. ただし, すぬけ君がどのようにマス目の色を変えてもけぬす君が $ (H,\ W) $ にたどり着くことが出来ない場合、$ -1 $ と出力しなさい.

## 输入输出样例 #1

### 输入 #1

```
3 3
..#
#..
...
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
10 37
.....................................
...#...####...####..###...###...###..
..#.#..#...#.##....#...#.#...#.#...#.
..#.#..#...#.#.....#...#.#...#.#...#.
.#...#.#..##.#.....#...#.#.###.#.###.
.#####.####..#.....#...#..##....##...
.#...#.#...#.#.....#...#.#...#.#...#.
.#...#.#...#.##....#...#.#...#.#...#.
.#...#.####...####..###...###...###..
.....................................
```

### 输出 #2

```
209
```

## 说明/提示

### 制約

- $ H $ は $ 2 $ 以上 $ 50 $ 以下の整数
- $ W $ は $ 2 $ 以上 $ 50 $ 以下の整数
- $ s_{i,\ j} $ は `.` または `#` $ (1\ \leq\ i\ \leq\ H,\ 1\ \leq\ j\ \leq\ W) $
- $ s_{1,\ 1},\ s_{H,\ W} $ は `.` である

### Sample Explanation 1

下の図のようにマス目の色を変えれば, スコア $ 2 $ を達成できます. !\[Explanation of Sample 1\](https://img.atcoder.jp/abc088/bc944898899615e35f898654b68cd517.png)