## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc013/tasks/agc013_d

joisinoお姉ちゃんは、大きな箱と、たくさんの赤い積み木と青い積み木を持っています。 joisinoお姉ちゃんは、次の手順にそって、これらの積み木を積み上げることにしました。

まず、赤い積み木と青い積み木を、合わせて $ N $ 個、箱に入れます。 合計で $ N $ 個ならば、それぞれの色の積み木の個数に制限はありません。 特に、一方の色の積み木の個数が $ 0 $ 個でも構いません。 次に、ある操作を $ M $ 回行います。 $ 1 $ 回の操作は、以下の $ 3 $ つのステップからなります。

- 好きな積み木を箱から $ 1 $ つ取り出す。
- 赤い積み木と青い積み木を $ 1 $ つずつ箱にいれる。
- 再び、好きな積み木を箱から $ 1 $ つ取り出す。

$ M $ 回の操作のあと、それまでに取り出した積み木を、取り出した順番に積み重ねます。 joisinoお姉ちゃんは、こうして積みあがる $ 2\ \times\ M $ 個の積み木の色の組み合わせが何通りあるか知りたくなりました。 あなたの仕事は、joisinoお姉ちゃんの代わりにこれを求めるプログラムを作ることです。 なお、答えは非常に大きくなることがあるので、$ 10^9+7 $ で割った余りを出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式
積み上がる積み木の色の組み合わせが何通りあるかを求め、$ 10^9+7 $ で割った余りを出力せよ。

## 题目大意
一开始有 $n$ 个颜色为黑白的球，但不知道黑白色分别有多少， $m$ 次操作，每次先拿出一个球，再放入黑白球各一个，再拿出一个球，最后拿出的球按顺序排列会形成一个颜色序列，求颜色序列有多少种。答案对 $10^9+7$ 取模。

$n,m$ 小于等于 $3000$。

```input1
2 3
```

```output1
56
```

```input2
1000 10
```

```output2
1048576
```

```input3
1000 3000
```

```output3
693347555
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 3000 $
- $ 1\ \leq\ M\ \leq\ 3000 $

### Sample Explanation 1

積み木を取り出すステップは合計で $ 6 $ 回行われます。 $ 2,3,4,5 $ 番目に取り出す積み木の色が全て同じになるような取り出し方だけがあり得ないので、 答えは、$ 2^6\ -\ 2\ \times\ 2\ \times\ 2\ =\ 56 $ となります。

