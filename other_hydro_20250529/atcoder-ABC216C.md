## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc216/tasks/abc216_c

空の箱があります。  
 髙橋君は以下の $ 2 $ 種類の魔法を好きな順番で好きな回数使えます。

- 魔法 $ A $ ：箱の中にボールを $ 1 $ つ増やす
- 魔法 $ B $ ：箱の中のボールの数を $ 2 $ 倍にする

合計 **$ \mathbf{120} $ 回以内**の魔法で、箱の中のボールの数をちょうど $ N $ 個にする方法を $ 1 $ つ教えてください。  
 なお、与えられた制約のもとで条件を満たす方法が必ず存在することが示せます。

魔法以外の方法でボールの数を変化させることはできません。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
`A` , `B` のみからなる文字列 $ S $ を出力せよ。  
 $ S $ の $ i $ 文字目が `A` ならば、髙橋君が $ i $ 回目に使う魔法が魔法 $ A $ であることを表し、`B` ならば魔法 $ B $ であることを表す。

$ S $ の長さは **$ \mathbf{120} $ 以下**でなければならない。

## 题目大意
### 题意

有一个空盒子。

你可以以任意顺序执行以下两种操作任意次：

- 操作 $A$ ：往盒子里放入一个球。
- 操作 $B$ ：使盒子里球的数量翻倍。

请输出一种**操作次数不超过 $120$ 的方案**使得盒子里有 $N$ 个球。

可以证明一定存在合法方案。

### 数据范围

- $1 \le N \le 10^{18}$
- 输入的所有数都是整数。

---

### 输入格式

输入一个整数 $N$ 。

### 输出格式

输出一个由 `A` 和 `B` 组成的字符串 $S$ ， $S$ 的第 $i$ 个字符表示第 $i$ 次操作的种类。

$S$ **至多由 $120$ 个字符**组成。

---


### 样例解释1

盒子中球数的变化情况为 $0 \xrightarrow{A} 1 \xrightarrow{A} 2 \xrightarrow{B} 4 \xrightarrow{A} 5$ 。

---



### 样例解释2

盒子中球数的变化情况为 $0 \xrightarrow{B} 0 \xrightarrow{B} 0 \xrightarrow{A} 1 \xrightarrow{B} 2 \xrightarrow{B} 4 \xrightarrow{A} 5 \xrightarrow{A} 6 \xrightarrow{A} 7 \xrightarrow{B} 14$ 。


$\textsf{Translated by @\color{5eb95e}nr0728}.$

```input1
5
```

```output1
AABA
```

```input2
14
```

```output2
BBABBAAAB
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^{18} $
- 入力は全て整数

### Sample Explanation 1

ボールの数は、$ 0\ \xrightarrow{A}\ 1\xrightarrow{A}\ 2\ \xrightarrow{B}4\xrightarrow{A}\ 5 $ と変化します。 `AAAAA` などの答えも正解になります。

### Sample Explanation 2

ボールの数は、$ 0\ \xrightarrow{B}\ 0\ \xrightarrow{B}\ 0\ \xrightarrow{A}1\ \xrightarrow{B}\ 2\ \xrightarrow{B}\ 4\ \xrightarrow{A}5\ \xrightarrow{A}6\ \xrightarrow{A}\ 7\ \xrightarrow{B}14 $ と変化します。 $ S $ の長さを最小化する必要はありません。

