## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc261/tasks/abc261_a

数直線があり、高橋君はこれを赤色と青色で次のように塗りました。

- $ X=L_1 $ から $ X=R_1 $ までをすべて赤色で塗る。
- $ X=L_2 $ から $ X=R_2 $ までをすべて青色で塗る。

数直線のうち、赤色と青色の両方で塗られている部分の長さを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ L_1 $ $ R_1 $ $ L_2 $ $ R_2 $

## 输出格式
両方の色で塗られている部分の長さを整数で出力せよ。

## 题目大意
题意：

高桥君将从$L_1$到$R_1$的部分涂成红色，将从$L_2$到$R_2$的部分涂成蓝色。


求同时涂有红色和蓝色的部分的长度。
 
### 注：即使红色和蓝色涂的部分相接，两种颜色涂的部分的长度也为0。

```input1
0 3 1 5
```

```output1
2
```

```input2
0 1 4 5
```

```output2
0
```

```input3
0 3 3 7
```

```output3
0
```

## 提示
### 制約

- $ 0\leq\ L_1\ <\ R_1\leq\ 100 $
- $ 0\leq\ L_2\ <\ R_2\leq\ 100 $
- 入力はすべて整数

### Sample Explanation 1

$ X=0 $ から $ X=3 $ までが赤く、 $ X=1 $ から $ X=5 $ までが青く塗られています。 よって、両方の色で塗られている部分は $ X=1 $ から $ X=3 $ までであり、その長さは $ 2 $ となります。

### Sample Explanation 2

両方の色で塗られている部分はありません。

### Sample Explanation 3

赤色と青色で塗られている部分が接している場合でも、 両方の色で塗られている部分の長さは $ 0 $ となります。

