## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc210/tasks/abc210_b

$ N $ 枚のカードからなる山札があります。  
 それぞれのカードは、「良いカード」か「悪いカード」かのどちらかです。

高橋君と青木君は、この山札を使って対戦ゲームをします。  
 このゲームでは、$ 2 $ 人は交互に山札の一番上のカードを引いて、そのカードを食べます。  
 先に悪いカードを食べたプレイヤーの負けです。（ここで、山札には少なくとも $ 1 $ 枚の悪いカードが含まれていることが保証されます。）

`0` と `1` からなる文字列 $ S $ が与えられます。$ i\ =\ 1,\ 2,\ \ldots,\ N $ について、

- $ S $ の $ i $ 文字目が `0` のとき、山札の上から $ i $ 番目のカードが良いカードであることを表します。
- $ S $ の $ i $ 文字目が `1` のとき、山札の上から $ i $ 番目のカードが悪いカードであることを表します。

高橋君が先手でゲームを始めるとき、高橋君と青木君の**どちらが負けるか**を答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式
高橋君が先手でゲームを始めるとき、高橋君と青木君の**どちらが負けるか**を答えよ。  
 高橋君が負けるならば `Takahashi` 、青木君が負けるならば `Aoki` と出力せよ。

## 题目大意
输入一个长为 $n$ 的 $01$ 串 $s$ ，求 $s$ 中从左往右数的第一个 $1$ 出现在第奇数个位置上还是第偶数个位置上（串中的第一个数为第 $1$ 位）。若在奇数位上输出Takahashi，否则输出Aoki。保证串中至少有一个 $1$ 。

```input1
5
00101
```

```output1
Takahashi
```

```input2
3
010
```

```output2
Aoki
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ N $ は整数
- $ S $ は `0` と `1` からなる長さ $ N $ の文字列
- $ S $ は少なくとも $ 1 $ 個の `1` を含む。

### Sample Explanation 1

まず、高橋君が良いカードを食べ、次に青木君が良いカードを食べ、その後に高橋君が悪いカードを食べます。 高橋君が先に悪いカードを食べるので高橋君が負けます。よって、`Takahashi` と出力します。

