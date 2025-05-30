## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc266/tasks/abc266_d

高橋君はすぬけ君たちを捕まえようとしています。

数直線上の座標 $ 0,1,2,3,4 $ の $ 5 $ 箇所に穴があり、すぬけ君たちの巣につながっています。

これから $ N $ 匹のすぬけ君が穴から出てきます。$ i $ 番目のすぬけ君は時刻 $ T_i $ に座標 $ X_i $ の穴から出てきて、大きさは $ A_i $ であることがわかっています。

高橋君は時刻 $ 0 $ に座標 $ 0 $ におり、数直線上を単位時間あたり $ 1 $ 以下の速さで移動することができます。  
すぬけ君が穴から出てきたのと同じ時刻に同じ座標に高橋君がいるとき、かつ、そのときに限り、高橋君はすぬけ君を捕まえることができます。  
すぬけ君を捕まえるのにかかる時間は無視できます。

高橋君が適切に行動したとき、捕まえることができるすぬけ君の大きさの合計の最大値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ T_1 $ $ X_1 $ $ A_1 $ $ T_2 $ $ X_2 $ $ A_2 $ $ \vdots $ $ T_N $ $ X_N $ $ A_N $

## 输出格式
答えを整数として出力せよ。

## 题目大意
高桥君在数轴上挖了 $5$ 个坑，坐标为 $0,1,2,3,4$。一开始他在 $0$ 位置，每秒最多移动 $1$ 单位。

现有 $n$ 条 Snuke，第 $i$ 条大小为 $A_i$，在第 $T_i$ 时刻出现在坐标为 $X_i$ 的坑。**请注意出现仅发生在瞬间，下一时刻消失。**

高桥君能抓到第 $i$ 条 Snuke 当且仅当某时刻他在第 $T_i$ 时刻出现在 $X_i$。请计算他抓到的 Snuke 总大小最大值。

```input1
3
1 0 100
3 3 10
5 4 1
```

```output1
101
```

```input2
3
1 4 1
2 4 1
3 4 1
```

```output2
0
```

```input3
10
1 4 602436426
2 1 623690081
3 3 262703497
4 4 628894325
5 3 450968417
6 1 161735902
7 1 707723857
8 2 802329211
9 0 317063340
10 2 125660016
```

```output3
2978279323
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 0\ <\ T_1\ <\ T_2\ <\ \ldots\ <\ T_N\ \leq\ 10^5 $
- $ 0\ \leq\ X_i\ \leq\ 4 $
- $ 1\ \leq\ A_i\ \leq\ 10^9 $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

次のように行動するのが最適です。 - 座標 $ 0 $ で待機し、時刻 $ 1 $ に $ 1 $ 番目のすぬけ君を捕まえる - 座標 $ 4 $ へ移動し、時刻 $ 5 $ に $ 3 $ 番目のすぬけ君を捕まえる $ 1 $ 番目と $ 2 $ 番目のすぬけ君を両方とも捕まえることはできないので、これが最大です。

### Sample Explanation 2

高橋君はすぬけ君を $ 1 $ 匹も捕まえることができません。

