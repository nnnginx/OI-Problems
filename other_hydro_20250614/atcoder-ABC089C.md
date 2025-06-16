## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc089/tasks/abc089_c

$ N $ 人の人がいて、$ i $ 番目の人の名前は $ S_i $ です。

この中から、以下の条件を満たすように $ 3 $ 人を選びたいです。

- 全ての人の名前が `M`,`A`,`R`,`C`,`H` のどれかから始まっている
- 同じ文字から始まる名前を持つ人が複数いない

これらの条件を満たすように $ 3 $ 人を選ぶ方法が何通りあるか、求めてください。ただし、選ぶ順番は考えません。

答えが $ 32 $ bit整数型に収まらない場合に注意してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ : $ $ S_N $

## 输出格式
与えられた条件を満たすように $ 3 $ 人を選ぶ方法が $ x $ 通りのとき、$ x $ を出力せよ。

## 题目大意
有 $N$ 个人，第 $i$ 个人的名字是 $S_i$。需要选择满足以下条件的三个人：

- 每个人的名字以 $M,A,R,C$ 或 $H$ 开头。
- 没有多个人的名字以相同的字母开头。

求一共有多少种方法可以选择三个人。

**注意：可能会爆 $int$，需要开 $long$ $long$**

```input1
5
MASHIKE
RUMOI
OBIRA
HABORO
HOROKANAI
```

```output1
2
```

```input2
4
ZZ
ZZZ
Z
ZZZZZZZZZZ
```

```output2
0
```

```input3
5
CHOKUDAI
RNG
MAKOTO
AOKI
RINGO
```

```output3
7
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ S_i $ は英大文字からなる
- $ 1\ \leq\ |S_i|\ \leq\ 10 $
- $ S_i\ \neq\ S_j\ (i\ \neq\ j) $

### Sample Explanation 1

次のような名前の $ 3 $ 人を選ぶと良いです。 - `MASHIKE`,`RUMOI`,`HABORO` - `MASHIKE`,`RUMOI`,`HOROKANAI` よって、$ 2 $ 通りとなります。

### Sample Explanation 2

与えられた条件を満たすように $ 3 $ 人を選ぶ方法が存在しない場合に注意してください。

