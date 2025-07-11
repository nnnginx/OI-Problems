# AT_zone2021_c MAD TEAM

## 题目描述

[problemUrl]: https://atcoder.jp/contests/zone2021/tasks/zone2021_c

$ N $ 人のメンバー候補がおり、それぞれの人は、パワー・スピード・テクニック・知識・発想力の $ 5 $ 種類の能力値を持っています。  
 $ i $ 番目の人のパワーは $ A_i $ 、スピードは $ B_i $ 、テクニックは $ C_i $ 、知識は $ D_i $ 、発想力は $ E_i $ です。  
 あなたは、$ N $ 人のメンバー候補から $ 3 $ 人を選び、$ 1 $ つのチームを作ります。  
 チーム全体のパワーをチームメンバーのパワーの最大値で定義します。スピード・テクニック・知識・発想力についても同様に定義します。  
 チームの総合力を、チーム全体のパワー・スピード・テクニック・知識・発想力の最小値で定義します。  
 チームの総合力としてありえる最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ C_1 $ $ D_1 $ $ E_1 $ $ A_2 $ $ B_2 $ $ C_2 $ $ D_2 $ $ E_2 $ $ \vdots $ $ A_N $ $ B_N $ $ C_N $ $ D_N $ $ E_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
3 9 6 4 6
6 9 3 1 1
8 8 9 3 7
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
5
6 13 6 19 11
4 4 12 11 18
20 7 19 2 5
15 5 12 20 7
8 7 6 18 5
```

### 输出 #2

```
13
```

## 输入输出样例 #3

### 输入 #3

```
10
6 7 5 18 2
3 8 1 6 3
7 2 8 7 7
6 3 3 4 7
12 8 9 15 9
9 8 6 1 10
12 9 7 8 2
10 3 17 4 10
3 1 3 19 3
3 14 7 13 1
```

### 输出 #3

```
10
```

## 说明/提示

### ストーリー

さて、本格的に UFO と対峙する仲間を集めることにしよう。それも、とびきり MAD で優秀な。  
 俺は数多の天才たちと競い合ってきた「AtCoder」上でメンバーを集めることにした。  
 名の知れたプログラマに片っ端から声をかけてもいいが、どうせなら得意分野のバランスが良い少数精鋭で最高なチームを作るとしよう。

### 制約

- 入力は全て整数
- $ 3\ <\ =\ N\ <\ =\ 3000 $
- $ 1\ <\ =\ A_i,\ B_i,\ C_i,\ D_i,\ E_i\ <\ =\ 10^9 $

### Sample Explanation 1

$ 3 $ 人全員をチームに入れるほかありません。 この時、チーム全体の各能力値は以下のようになります。 - チーム全体のパワー : $ \max(3,\ 6,\ 8)\ =\ 8 $ - チーム全体のスピード : $ \max(9,\ 9,\ 8)\ =\ 9 $ - チーム全体のテクニック : $ \max(6,\ 3,\ 9)\ =\ 9 $ - チーム全体の知識 : $ \max(4,\ 1,\ 3)\ =\ 4 $ - チーム全体の発想力 : $ \max(6,\ 1,\ 7)\ =\ 7 $ したがって、チームの総合力は $ \min(8,\ 9,\ 9,\ 4,\ 7)\ =\ 4 $ となります。

### Sample Explanation 2

$ 1,\ 2,\ 3 $ 番目の人を採用すると、チームの総合力は $ \min(20,\ 13,\ 19,\ 19,\ 18)\ =\ 13 $ です。