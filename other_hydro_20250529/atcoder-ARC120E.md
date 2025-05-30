## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc120/tasks/arc120_e

人 $ 1 $ から人 $ N $ までの $ N $ 人の人が数直線上に並んでいます。人 $ i $ は今数直線上の座標 $ A_i $ にいます。  
 ここで、$ A_1\ <\ A_2\ <\ A_3\ <\ \dots\ <\ A_N $ であり、$ A_i $ は全て偶数です。

今から $ k $ 秒間のパーティーを開きます。  
 パーティー中、各人は毎秒 $ 1 $ 以下の速さで数直線上を自由に動くことができます。(速さが毎秒 $ 1 $ 以下であれば負の向きに動くこともできます。)  
 参加者の希望により、$ 1\ \le\ i\ \lt\ N $ を満たす全ての整数 $ i $ について以下の条件を満たす必要があります。

- 人 $ i $ と人 $ i\ +\ 1 $ が同じ座標にいる瞬間が、パーティー中 (終了の瞬間も含む) に少なくとも $ 1 $ 回存在する

各人が最適に行動すると条件を全て満たすことができるような最小の $ k $ を求めてください。  
 この問題の制約下で答えが整数になることが証明できます。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ A_3 $ $ \dots $ $ A_N $

## 输出格式
答えを整数として出力せよ。

## 题目大意
### 题目描述
有 $ N $ 个人打算开派对，他们均分布在数轴上，编号从 $1$ 到 $N$，第 $i$ 个人位于 $ a_i $ 点。初始是他们都位于数轴上不同的点。具体的，所有人所在的点都是偶数点，且有 $ a_1 < a_2 < a_3 <\cdots< a_n$。

派对计划进行 $k$ 秒，每个人每秒钟可以在数轴上向左或者向右移动一个单位长度，也可以不移动。

我们都知道，开派对至少要两个人。所以派对成功举行的条件是，对于任意的某个人 $j (1≤j<N)$，经过一系列移动过程，在派对进行中至少有一瞬间（包括派对结束的那一刻）使得 $a_j = a_{j+1}$（以当前那一秒结束时的位置为准）。

请计算能够使得派对成功举行的最小的 $k$。

能够证明在题目限定条件下答案一定存在。

### 输入格式

第一行一个正整数 $N$。  
第二行包含 $ N $ 个正整数表示 $a_i$。

### 输出格式

一行一个整数，表示满足条件的最小 $k$ 值。

### 样例解释

#### 样例 1 解释

我们依次把 $3$ 个人记为 $A,B,C$，在 $5$ 秒内，每个人可以进行如下方式的移动：

- $A$ 一直向右移动； 
- $B$ 前 $2$ 秒向右移动，后 $3$ 秒向左移动； 
- $C$ 一直向左移动。

这样 $B$ 和 $C$ 在第 $2$ 秒结束时到达同一个位置，$A$ 和 $B$ 在第 $5$ 秒结束时到达同一个位置。

#### 样例 2 解释

我们依次把 $5$ 个人记为 $A,B,C,D,E$。

- $A$ 一直向右移动；
- $B$ 前 $2$ 秒向右移动，后 $1$ 秒向左移动；
- $C$ 一直保持不动；
- $D$ 前 $2$ 秒向左移动，后 $1$ 秒向右移动； 
- $E$ 一直向左移动；

这样 $(B,C),(C,D)$ 同时在第 $2$ 秒结束时到达同一个位置，$(A,B),(D,E)$ 分别在第 $3$ 秒结束时到达同一个位置。

```input1
3
0 6 10
```

```output1
5
```

```input2
5
0 2 4 6 8
```

```output2
3
```

```input3
10
0 2 4 6 8 92 94 96 98 100
```

```output3
44
```

## 提示
### 制約

- $ 2\ \le\ N\ \le\ 2\ \times\ 10^5 $
- $ 0\ \le\ A_i\ \le\ 10^9 $
- $ A_1\ <\ A_2\ <\ A_3\ <\ \dots\ <\ A_N $
- $ A_i $ は偶数

### Sample Explanation 1

$ 5 $ 秒間のパーティーの間、各人は以下のように移動するとよいです。 - 人 $ 1 $ : 常に正の向きに速さ $ 1 $ で移動する - 人 $ 2 $ : 最初の $ 2 $ 秒間は正の向きに速さ $ 1 $ で移動し、残りの $ 3 $ 秒間は負の向きに速さ $ 1 $ で移動する - 人 $ 3 $ : 常に負の向きに速さ $ 1 $ で移動する 各人がこのように移動した場合、開始からちょうど $ 2 $ 秒後に人 $ 2 $ と人 $ 3 $ が同じ座標にいます。また、パーティーの終了時に人 $ 1 $ と人 $ 2 $ が同じ座標にいます。 よって、$ k\ =\ 5 $ の場合、条件を全て満たすことができます。これより小さい $ k $ では条件を全て満たすような移動の仕方は存在しません。

### Sample Explanation 2

$ 3 $ 秒間のパーティーの間、各人は例えば以下のように移動するとよいです。 - 人 $ 1 $ : 常に正の向きに速さ $ 1 $ で移動する - 人 $ 2 $ : 最初の $ 2 $ 秒間は正の向きに速さ $ 1 $ で移動し、残りの $ 1 $ 秒間は負の向きに速さ $ 1 $ で移動する - 人 $ 3 $ : 常に移動しない - 人 $ 4 $ : 最初の $ 2 $ 秒間は負の向きに速さ $ 1 $ で移動し、残りの $ 1 $ 秒間は正の向きに速さ $ 1 $ で移動する - 人 $ 5 $ : 常に負の向きに速さ $ 1 $ で移動する

