## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc260/tasks/abc260_b

入学試験の受験者が $ N $ 人います。  
 試験の結果、 $ i $ 番の受験生は数学で $ A_i $ 点、英語で $ B_i $ 点を取りました。

試験の合格者は次のように決められます。

1. 数学の点が高い方から $ X $ 人を合格とする。
2. 次に、この時点でまだ合格となっていない受験者のうち、英語の点が高い方から $ Y $ 人を合格とする。
3. 次に、この時点でまだ合格となっていない受験者のうち、数学と英語の合計点が高い方から $ Z $ 人を合格とする。
4. ここまでで合格となっていない受験者は、不合格とする。

ただし、 1. から 3. までのどの段階についても、同点であった場合は受験生の番号の小さい方を優先します。入出力例も参照してください。

以上の手順で合格者を決める時、合格となった受験生の番号を小さい方から順に改行区切りで出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $ $ Y $ $ Z $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $ $ B_1 $ $ B_2 $ $ \dots $ $ B_N $

## 输出格式
合格となった受験生の番号を小さい方から順に改行区切りで出力せよ。

## 题目大意
一次入学考试后，第 $i$ 个学生的数学成绩是 $A_i$，英语成绩是 $B_i$,考试合格者的决定如下：


1. 以数学分数高的前 $X$ 人为合格。 
2. 接着，在还没有合格的应试者中，以英语分数高的前 $Y$ 者为合格。 
3. 接着，在此时还未合格的应试者中，以数学和英语合计分数高的前 $Z$ 人为合格。 
4. 到此为止还未合格的考生，视为不合格。 

如果分数一样，则编号小的学生优先。
从小到大输出及格的学生编号。

```input1
6 1 0 2
80 60 80 60 70 70
40 20 50 90 90 80
```

```output1
1
4
5
```

```input2
5 2 1 2
0 100 0 100 0
0 0 100 100 0
```

```output2
1
2
3
4
5
```

```input3
15 4 3 2
30 65 20 95 100 45 70 85 20 35 95 50 40 15 85
0 25 45 35 65 70 80 90 40 55 20 20 45 75 100
```

```output3
2
4
5
6
7
8
11
14
15
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ \le\ N\ \le\ 1000 $
- $ 0\ \le\ X,Y,Z\ \le\ N $
- $ 1\ \le\ X+Y+Z\ \le\ N $
- $ 0\ \le\ A_i,B_i\ \le\ 100 $

### Sample Explanation 1

\- まず、数学の点が高い方から $ 1 $ 人が合格となります。 - 数学の最高点は $ 80 $ 点で $ 1 $ 番の受験生と $ 3 $ 番の受験生が並んでいますが、受験生の番号が小さい方が優先され $ 1 $ 番の受験生が合格となります。 - 次に、まだ合格となっていない受験者のうち、英語の点が高い方から $ 0 $ 人が合格となります。 - 明らかに、ここで合格者が増えることはありません。 - 次に、まだ合格となっていない受験者のうち、数学と英語の合計点が高い方から $ 2 $ 人が合格となります。 - まず、まだ合格となっていない受験者の中で、合計点が $ 160 $ 点と最も高い $ 5 $ 番の受験生が合格となります。 - 次に、まだ合格となっていない受験者の中で、合計点が $ 150 $ 点の $ 4 $ 番の受験生と $ 6 $ 番の受験生が並んでいます。受験生の番号の小さい方が優先され、 $ 4 $ 番の受験生が合格となります。 以上より、合格となる受験生の番号は $ 1,4,5 $ なので、小さい方から出力してください。

### Sample Explanation 2

全員が合格となることもあります。

