# AT_abc351_a [ABC351A] The bottom of the ninth

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc351/tasks/abc351_a

チーム高橋とチーム青木が、チーム高橋を先攻として野球を行なっています。  
現在、$ 9 $ 回表までが終了し、$ 9 $ 回裏が始まろうとしています。

試合において、チーム高橋は $ i $ 回表 $ (1\leq\ i\leq\ 9) $ に $ A_i $ 点を取り、チーム青木は $ j $ 回裏 $ (1\leq\ j\leq\ 8) $ に $ B_j $ 点を取りました。  
ここで、$ 9 $ 回表の終了時点でチーム高橋の得点はチーム青木の得点以上です。  
チーム青木は $ 9 $ 回裏に最低何点取れば勝利することができるか求めてください。

ただし、$ 9 $ 回裏の終了時点で同点であった場合は引き分けとなり、すなわちチーム青木が勝利するためには $ 9 $ 回裏の終了時点でチーム高橋より真に多くの点をとっている必要があるものとします。  
なお、（ある時点における）チーム高橋の得点はそれまでの回の表に取った点数の合計であり、チーム青木の得点はそれまでの回の裏に取った点数の合計です。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A_1 $ $ A_2 $ $ A_3 $ $ A_4 $ $ A_5 $ $ A_6 $ $ A_7 $ $ A_8 $ $ A_9 $ $ B_1 $ $ B_2 $ $ B_3 $ $ B_4 $ $ B_5 $ $ B_6 $ $ B_7 $ $ B_8 $

## 输出格式

チーム青木が勝利するために $ 9 $ 回裏に取る必要のある最小の得点を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
0 1 0 1 2 2 0 0 1
1 1 0 0 0 0 1 0
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0
```

### 输出 #2

```
1
```

## 说明/提示

### 制約

- $ 0\leq\ A_i,\ B_j\leq\ 99 $
- $ A_1\ +\ A_2\ +\ A_3\ +\ A_4\ +\ A_5\ +\ A_6\ +\ A_7\ +\ A_8\ +\ A_9\ \geq\ B_1\ +\ B_2\ +\ B_3\ +\ B_4\ +\ B_5\ +\ B_6\ +\ B_7\ +\ B_8 $
- 入力はすべて整数

### Sample Explanation 1

$ 9 $ 回表の終了時点でチーム高橋の得点は $ 7 $ 点、チーム青木の得点は $ 3 $ 点となっています。 よって、チーム青木は$ 9 $ 回裏に $ 5 $ 点取れば $ 7-8 $ となり、勝利することができます。 $ 9 $ 回裏に $ 4 $ 点では、引き分けとなり勝利できないことに注意してください。