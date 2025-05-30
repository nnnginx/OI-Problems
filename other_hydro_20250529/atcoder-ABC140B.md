## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc140/tasks/abc140_b

高橋くんは $ N $ 種類の料理が食べ放題のビュッフェに行き、全種類の料理 (料理 $ 1 $, 料理 $ 2 $, $ \ldots $, 料理 $ N $) を $ 1 $ 度ずつ食べました。

高橋くんが $ i $ $ (1\ \leq\ i\ \leq\ N) $ 番目に食べた料理は料理 $ A_i $ でした。

高橋くんは、料理 $ i $ $ (1\ \leq\ i\ \leq\ N) $ を食べると満足度 $ B_i $ を得ます。

また、料理 $ i $ $ (1\ \leq\ i\ \leq\ N\ -\ 1) $ を食べた直後に料理 $ i+1 $ を食べると満足度 $ C_i $ を追加で得ます。

高橋くんが得た満足度の合計を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ ... $ $ A_N $ $ B_1 $ $ B_2 $ $ ... $ $ B_N $ $ C_1 $ $ C_2 $ $ ... $ $ C_{N-1} $

## 输出格式
高橋くんが得た満足度の合計を整数で出力せよ。

## 题目大意
### 题目描述

一天，高桥去吃自助餐。自助餐厅一共有 $n$ 种菜肴，第 $i$ 种菜肴简称菜肴 $i$。高桥把每种菜肴都吃了一遍。已知高桥是按照（菜肴 $a_1$，菜肴 $a_2$，...，菜肴 $a_n$）的顺序吃的，且他每吃完菜肴 $i$ 就会获得一个满足值 $b_i$。同时，如果他在吃完菜肴 $i$ 之后立刻吃菜肴 $i+1$，那么他的满足值就会在原来的基础上追加一个值 $c_i$。现在给出上文所述的全部信息，请求出高桥在吃完这 $n$ 种菜肴后的满足值之和。

### 输入格式

输入共 $4$ 行。第一行输入一行一个正整数 $n$，第二行按照 $i=1,2,...,n$ 的顺序输入高桥吃的第 $i$ 道菜的编号 $a_i$，第三行按照 $i=1,2,...,n$ 的顺序输入高桥在吃完第 $i$ 道菜之后能获得的满足值 $b_i$，第四行按照 $i=1,2,...,n-1$ 的顺序输入高桥在吃完第 $i$ 道菜之后立即吃第 $i+1$ 道菜时追加的满足值 $c_i$。

### 输出格式

输出一行一个正整数，即高桥在吃完全部 $n$ 道菜之后获得的满足值之和。

### 说明/提示

**【输入输出样例 #1 解释】**

高桥先吃第 $3$ 道菜，获得满足值 $4$；他接着吃第 $1$ 道菜，获得满足值 $2$；最后他吃了第 $2$ 道菜，获得满足值 $5$。由于 $2=1+1$，所以吃完最后一道菜后追加满足值 $3$。高桥共计获得满足值 $4+2+5+3=14$.

**数据规模与约定**

对于全部测试点，数据保证：

- $2 \le n \le 20$；
- $1 \le a_i \le n$ 且 $a_i$ 互不相同；
- $1 \le b_i,c_i \le 50$；
- 所有输入数据均为整数。

```input1
3
3 1 2
2 5 4
3 6
```

```output1
14
```

```input2
4
2 3 4 1
13 5 8 24
45 9 15
```

```output2
74
```

```input3
2
1 2
50 50
50
```

```output3
150
```

## 提示
### 制約

- 入力は全て整数である。
- $ 2\ \leq\ N\ \leq\ 20 $
- $ 1\ \leq\ A_i\ \leq\ N $
- $ A_1,\ A_2,\ ...,\ A_N $ は全て異なる。
- $ 1\ \leq\ B_i\ \leq\ 50 $
- $ 1\ \leq\ C_i\ \leq\ 50 $

### Sample Explanation 1

以下のように高橋くんは合計 $ 14 $ の満足度を得ました。 - 高橋くんはまず料理 $ 3 $ を食べ、満足度 $ 4 $ を得ました。 - 高橋くんは次に料理 $ 1 $ を食べ、満足度 $ 2 $ を得ました。 - 高橋くんは最後に料理 $ 2 $ を食べ、満足度 $ 5\ +\ 3\ =\ 8 $ を得ました。

