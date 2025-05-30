## 题目描述
[problemUrl]: https://atcoder.jp/contests/tenka1-2019/tasks/tenka1_2019_c

$ N $ 個の石が一列に並んでおり、すべての石は白か黒で塗られています。 石の状態は長さ $ N $ の文字列 $ S $ で表され、$ S $ の $ i $ 文字目が `.` のとき左から $ i $ 個目の石が白であり、`#` のとき左から $ i $ 個目の石が黒であることを表します。

高橋君は、$ 0 $ 個以上の石の色を黒または白に変更し、黒い石のすぐ右に白い石があるような箇所がないようにしたいです。 色を変更する必要のある石の個数の最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式
色を変更する必要のある石の個数の最小値を出力せよ。

## 题目大意
有 N 块石头连续排列，每块石头都被漆成白色或黑色。 字符串 S 代表石头的颜色。 如果 S 的第i个字符是 `.`，则从左起第 i 个石头是白色；如果字符是 `＃`，则第 i 个石头是黑色。

高桥希望将某些石头的颜色更改为黑色或白色，以使黑色石头的右侧不会立即出现白色石头。 找到需要重新着色的最少数量的石头。

```input1
3
#.#
```

```output1
1
```

```input2
5
#.##.
```

```output2
2
```

```input3
9
.........
```

```output3
0
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ S $ は `.`, `#` のみからなる長さ $ N $ の文字列である

### Sample Explanation 1

例えば、$ 1 $ 個目の石の色を白に変更すればよいです。

