## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc221/tasks/abc221_d

あるオンラインゲームがあり、 $ N $ 人のプレイヤーが登録しています。  
 サービス開始日から $ 10^{100} $ 日を迎えた今日、 開発者である高橋君がログイン履歴を調べたところ、 $ i $ 番目のプレイヤーはサービス開始日を $ 1 $ 日目として、 $ A_i $ 日目から $ B_i $ 日間連続でログインし、 それ以外の日はログインしていなかったことが判明しました。 すなわち、$ i $ 番目のプレイヤーはサービス開始日から、$ A_i $ , $ A_i+1 $ , $ \ldots $ , $ A_i+B_i-1 $ 日目に、 かつそれらの日にのみログインしていたことが分かりました。  
 $ 1\leq\ k\leq\ N $ をみたす各整数 $ k $ について、 サービス開始日から今日までの間で、ちょうど $ k $ 人がログインしていた日数を答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ : $ $ A_N $ $ B_N $

## 输出格式
次のように空白区切りで $ N $ 個の整数を出力せよ。

> $ D_1 $ $ D_2 $ $ \cdots $ $ D_N $

ただし、 $ D_i $ はちょうど $ i $ 人がゲームにログインしていた日数を表す。

## 题目大意
高桥是一款电子游戏的开发者。

在这款游戏上线 $\inf$ 天后，高桥打开了操作记录，查看了所有 $n$ 个玩家的入坑时间以及总共玩的天数。

现在要，对于每一个整数 $k$ 使 $1\le k\le n$ ，有多少天有**恰好** $k$ 个玩家正在玩这个游戏。

```input1
3
1 2
2 3
3 1
```

```output1
2 2 0
```

```input2
2
1000000000 1000000000
1000000000 1000000000
```

```output2
0 1000000000
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^9 $
- $ 1\ \leq\ B_i\ \leq\ 10^9 $
- 入力は全て整数である。

### Sample Explanation 1

$ 1 $ 番目のプレイヤーは $ 1 $ 日目と $ 2 $ 日目に、 $ 2 $ 番目のプレイヤーは $ 2 $ 日目と $ 3 $ 日目と $ 4 $ 日目に、 $ 3 $ 番目のプレイヤーは $ 3 $ 日目だけにログインしています。 よって、$ 1 $, $ 4 $ 日目には $ 1 $ 人が、$ 2 $, $ 3 $ 日目には $ 2 $ 人がログインしており、 それ以外の日は誰もログインしていない事が分かります。 答えはちょうど $ 1 $ 人がログインした日数が $ 2 $ 日、 ちょうど $ 2 $ 人がログインした日数が $ 2 $ 日、 ちょうど $ 3 $ 人がログインした日数が $ 0 $ 日となります。

### Sample Explanation 2

$ 2 $ 人以上のプレイヤーがちょうど同じ期間にログインしていることもあり得ます。

