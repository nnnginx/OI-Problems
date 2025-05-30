## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc242/tasks/abc242_a

あるプログラミングコンテストでは、以下のルールに従って参加者に T シャツをプレゼントします。

- 上位 $ A $ 位までの参加者は、必ず T シャツが貰える。
- 加えて、上位 $ A+1 $ 位から $ B $ 位までの参加者のうち $ C $ 人が一様ランダムに選ばれ、選ばれた参加者は T シャツを貰える。

コンテストには $ 1000 $ 人が参加し、全ての参加者が相異なる順位を取りました。  
 このコンテストの参加者であるいろはちゃんは、$ X $ 位を取りました。  
 このとき、いろはちゃんが T シャツを貰える確率を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ X $

## 输出格式
答えを出力せよ。 なお、想定解との絶対誤差または相対誤差が $ 10^{−6} $ 以下であれば、正解として扱われる。

## 题目大意
共 $1000$ 位选手参加比赛，前 $A$ 位选手必得奖，第 $A+1$ 到 $B$ 名随机选 $C$ 位选手得奖，在每个人排名都不同的情况下第 $X$ 名得到奖的概率是多少。

答案误差在 $10^{-6}$ 一下判为正确。

Translated by ShanCreeper.

```input1
30 500 20 103
```

```output1
0.042553191489
```

```input2
50 500 100 1
```

```output2
1.000000000000
```

```input3
1 2 1 1000
```

```output3
0.000000000000
```

## 提示
### 制約

- 入力はすべて整数
- $ 1\ \le\ A\ <\ B\ \le\ 1000 $
- $ 1\ \le\ C\ \le\ B-A $
- $ 1\ \le\ X\ \le\ 1000 $

### Sample Explanation 1

いろはちゃんは $ 103 $ 位を取りました。 $ 31 $ 位から $ 500 $ 位までの $ 470 $ 人の参加者の中から $ 20 $ 人が一様ランダムに選ばれ、ここで選ばれるといろはちゃんは T シャツを貰えます。この確率は $ \frac{20}{470}=0.04255319\dots $ です。

### Sample Explanation 2

いろはちゃんは $ 1 $ 位を取りました。この入力において、いろはちゃんは確実に T シャツを貰えます。

### Sample Explanation 3

いろはちゃんは $ 1000 $ 位を取りました。この入力において、いろはちゃんが T シャツを貰えることはありません。

