## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc119/tasks/arc119_d

$ H $ 行 $ W $ 列のマス目で表されるキャンバスがあり、上から $ i $ $ (1\ \leq\ i\ \leq\ H) $ 行目・左から $ j $ $ (1\ \leq\ j\ \leq\ W) $ 列目のマスを $ (i,\ j) $ と表します。最初、マス $ (i,\ j) $ は $ s_{i,\ j}= $ `R` のとき赤色で、$ s_{i,\ j}= $ `B` のとき青色で塗られています。

あなたは「次の $ 2 $ つのうち一方を選んで操作すること」を何回でも行うことができます。

> **操作X** 赤色で塗られているマスを $ 1 $ つ選び、そのマスと同じ行にあるすべてのマス（自分自身を含む）を白色に塗り替える。  
> **操作Y** 赤色で塗られているマスを $ 1 $ つ選び、そのマスと同じ列にあるすべてのマス（自分自身を含む）を白色に塗り替える。

最終的に白色で塗られたマスの個数を最大にするような、操作手順の一例を示してください。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ H $ $ W $ $ s_{1,\ 1} $$ s_{1,\ 2} $$ s_{1,\ 3} $$ \cdots $$ s_{1,\ W} $ $ s_{2,\ 1} $$ s_{2,\ 2} $$ s_{2,\ 3} $$ \cdots $$ s_{2,\ W} $ $ s_{3,\ 1} $$ s_{3,\ 2} $$ s_{3,\ 3} $$ \cdots $$ s_{3,\ W} $ $ \vdots $ $ s_{H,\ 1} $$ s_{H,\ 2} $$ s_{H,\ 3} $$ \cdots $$ s_{H,\ W} $

## 输出格式
以下の形式で、標準出力に出力してください。

> $ n $ $ t_1 $ $ r_1 $ $ c_1 $ $ t_2 $ $ r_2 $ $ c_2 $ $ t_3 $ $ r_3 $ $ c_3 $ $ \vdots $ $ t_n $ $ r_n $ $ c_n $

ここで、$ n $ は操作を行う回数、$ t_i,\ r_i,\ c_i $ $ (1\ \leq\ i\ \leq\ n) $ は「$ i $ 回目にはマス $ (r_i,\ c_i) $ を選び操作 $ t_i $ を行うこと」を表しています。  
 $ t_i $ は `X` または `Y` でなければなりません。  
 なお、複数通りの答えが考えられる場合は、そのどれを出力しても構いません。

## 题目大意
$H\times W$ 的网格，每个格子要么是蓝色（`B`）,要么是红色（`R`）。选择一个红色格子将其一行或一列涂白，请给出一个使得白色格子最多的方案。

样例1解释：

![样例解释](https://vj.csgrandeur.cn/225d2cc17dd2911a9a132b90d817503c?v=1688564646)

```input1
4 4
RBBB
BBBB
BBBB
RBRB
```

```output1
3
X 1 1
Y 4 3
X 4 1
```

```input2
1 119
BBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBBBBBRBBB
```

```output2
4
Y 1 60
Y 1 109
Y 1 46
X 1 11
```

```input3
10 10
BBBBBBBBBB
BBBBBBBBBB
BBBBBBBBBB
BBBBBBBBBB
BBBBBBBBBB
BBBBBBBBBB
BBBBBBBBBB
BBBBBBBBBB
BBBBBBBBBB
BBBBBBBBBB
```

```output3
0
```

## 提示
### 制約

- $ 1\ \leq\ H\ \leq\ 2500 $
- $ 1\ \leq\ W\ \leq\ 2500 $
- $ s_{i,\ j} $ は `R` または `B` である $ (1\ \leq\ i\ \leq\ H,\ 1\ \leq\ j\ \leq\ W) $
- $ H,\ W $ は整数

### Sample Explanation 1

たとえば次のように操作を行うことで、$ 10 $ 個のマスを白色にすることができます。 - まず、マス $ (1,\ 1) $ を選び、\*\*操作X\*\*を行う。 - 次に、マス $ (4,\ 3) $ を選び、\*\*操作Y\*\*を行う。 - 次に、マス $ (4,\ 1) $ を選び、\*\*操作X\*\*を行う。 なお、$ 11 $ 個以上のマスを白色にする方法は存在しません。 !\[ \](https://img.atcoder.jp/arc119/b0fde87f879b9dc90ca8788945f21bf2.png)

### Sample Explanation 2

すべてのマスを白色に塗り替えることができます。

### Sample Explanation 3

赤色のマスが $ 1 $ つも存在しないため、そもそも操作を行うことができません。

