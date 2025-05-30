## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc034/tasks/agc034_a

$ N $ 個の一列に並んだマス目があり、左から順に番号 $ 1,\ 2,\ ...,\ N $ がついています。長さ $ N $ の `.`, `#` からなる文字列 $ S $ が与えられ、$ S $ の $ i $ 文字目が `#` のときマス目 $ i $ には岩が置かれており、$ S $ の $ i $ 文字目が `.` のときマス目 $ i $ には何も置かれていません。

最初、マス目 $ A $ にすぬけ君、$ B $ にふぬけ君がいます。

あなたは以下の操作を好きなだけ繰り返すことができます。

- すぬけ君かふぬけ君を選び、$ 1 $ マス右か $ 2 $ マス右にジャンプさせる。このときジャンプ先にマスが存在しなければならず、またそのマスに岩が置かれていたりもう一人がいてはならない。

あなたはこの操作を繰り返し、マス目 $ C $ にすぬけ君が、$ D $ にふぬけ君がいるようにしたいです。

このようなことが可能かどうかを判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A $ $ B $ $ C $ $ D $ $ S $

## 输出格式
題意が達成可能ならば `Yes`、不可能ならば `No` を出力せよ。

## 题目大意
有一排 $n$ 个格子，编号为 $1,2,...n$，每个格子为 `#`（障碍）或者 `.`（可停留处）

有两个棋子，初始位置为 $A,B$，分别将其移动到 $C,D$ 两个格子上。

要求：
- 棋子每次跳 $1$ 或 $2$ 步，只能向右移。
- 不可以在障碍处停留，不能跳到已经有棋子的格子。

求：能否使 $A$ 中的棋子最终到达 $C$，$B$ 中的棋子最终到达 $D$。

保证 $A<B,A<C,B<D$。

```input1
7 1 3 6 7
.#..#..
```

```output1
Yes
```

```input2
7 1 3 7 6
.#..#..
```

```output2
No
```

```input3
15 1 3 15 13
...#.#...#.#...
```

```output3
Yes
```

## 提示
### 制約

- $ 4\ \leq\ N\ \leq\ 200,000 $
- $ S $ は `.`, `#` からなる長さ $ N $ の文字列
- $ 1\ \leq\ A,\ B,\ C,\ D\ \leq\ N $
- マス目 $ A,\ B,\ C,\ D $ に岩は置かれていない
- $ A,\ B,\ C,\ D $ はすべて異なる
- $ A\ <\ B $
- $ A\ <\ C $
- $ B\ <\ D $

### Sample Explanation 1

たとえば、以下のように移動させれば良いです(すぬけ君、ふぬけ君を `A`, `B` で表します) ``` A#B.#.. A#.B#.. .#AB#.. .#A.#B. .#.A#B. .#.A#.B .#..#AB ```

