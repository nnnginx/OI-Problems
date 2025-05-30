## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc139/tasks/abc139_b

高橋くんの家には電源プラグの差込口が $ 1 $ 口しかありません。

そこで、高橋くんは $ A $ 個口の電源タップをいくつか使って未使用の差込口を $ B $ 口以上に拡張したいと考えています。

$ A $ 個口の電源タップ $ 1 $ つと未使用の差込口 $ 1 $ 口を使って、新たに差込口を $ A $ 口増やすことができます。

最小でいくつの電源タップが必要でしょうか。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $

## 输出格式
必要な電源タップの個数の最小値を出力せよ。

## 题目大意
众所周知，坐长途火车是种煎熬，咕噜噜提前知道了：他所在卧铺的附近有且只有一个插座，但是他有 $N(1\leq N\leq 20)$ 个设备要充电。于是机智的咕噜噜想到了用插板来进行扩展。

已知每个插板可以扩展 $M(2\leq M\leq 20)$ 个插座，咕噜噜懒得算要准备多少个插板了，因此他想让你告诉他最少需要多少个插板。（咕噜噜好穷哦）

```input1
4 10
```

```output1
3
```

```input2
8 9
```

```output2
2
```

```input3
8 8
```

```output3
1
```

## 提示
### 制約

- 入力は全て整数である。
- $ 2\ \leq\ A\ \leq\ 20 $
- $ 1\ \leq\ B\ \leq\ 20 $

### Sample Explanation 1

$ 4 $ 個口の電源タップを $ 3 $ つ使うと、未使用の差込口は $ 10 $ 口になります。

### Sample Explanation 2

$ 8 $ 個口の電源タップを $ 2 $ つ使うと、未使用の差込口は $ 15 $ 口になります。

