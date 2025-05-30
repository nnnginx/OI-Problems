## 题目描述
[problemUrl]: https://atcoder.jp/contests/sumitrust2019/tasks/sumitb2019_e

$ N $ 人の人が一列に並んでおり、前から順に $ 1,\ 2,\ 3,\ ...,\ N $ と番号が付けられています。それぞれの人は、赤色・青色・緑色のいずれかの帽子を被っています。

さて、番号 $ i $ の人は以下の発言をしました。

- 「自分より前に、自分と同じ色の帽子を被っている人はちょうど $ A_i $ 人いる。」

すべての人の発言が正しいとして、$ N $ 人の人の帽子の色の組合せとして考えられるものが何通りあるか求めてください。

ただし、答えがとても大きくなる場合があるので、代わりに $ 1000000007 $ で割った余りを計算してください。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ N $ $ A_1 $ $ A_2 $ $ A_3 $ $ ... $ $ A_N $

## 输出格式
$ N $ 人の帽子の色の組合せとして考えられるものの個数を $ 1000000007 $ で割った余りを出力してください。

## 题目大意
$N$ 个人站成一列，每个人都戴着一顶帽子，颜色为红、黄、绿的一种。第 $i$ 个人前面有 $a_i$ 个人戴着和他颜色相同的帽子。求出 $N$ 个人帽子颜色的所有组合方案。

答案对 $10^9+7$ 取模。

- $1\leq N \leq 100000$
- $0\leq a_i \leq N-1$
- $N$ 和 $a_i$ 均为整数。

```input1
6
0 1 2 3 4 5
```

```output1
3
```

```input2
3
0 0 0
```

```output2
6
```

```input3
54
0 0 1 0 1 2 1 2 3 2 3 3 4 4 5 4 6 5 7 8 5 6 6 7 7 8 8 9 9 10 10 11 9 12 10 13 14 11 11 12 12 13 13 14 14 15 15 15 16 16 16 17 17 17
```

```output3
115295190
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100000 $
- $ 0\ \leq\ A_i\ \leq\ N-1 $
- 入力中の値はすべて整数

### Sample Explanation 1

以下の $ 3 $ 通りの組合せが考えられます。 - 赤, 赤, 赤, 赤, 赤, 赤 - 青, 青, 青, 青, 青, 青 - 緑, 緑, 緑, 緑, 緑, 緑

