# AT_abc009_2 [ABC009B] 心配性な富豪、ファミリーレストランに行く。

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc009/tasks/abc009_2

私は富豪だ。それも大富豪と言っていいぐらいお金を持っている。欲しいと思ったものはまずこの有り余るお金を使って買うことができる。しかし、この底の尽きないように思えるほどのお金でさえ人の心を買うことはできない。いくらお金があろうとも、ひとたび多くの庶民の反発を買ってしまえば、これまでのように生きていくことは難しくなるだろう。

この度私は庶民の気持ちを理解するため、初めてファミリーレストランという場所を訪れた。メニューを広げ、料理の内容とその金額を確かめると、なるほど驚きの安さである。どの料理の金額も取るに足らないようなものだから、とりあえず最も金額が高いものを選ぼうかと考えた。

しかし、考えてみれば、私は何のためにファミリーレストランに来たのであったか。庶民の気持ちを理解しようというのに、金額のことを考えずに最も高いものを選ぼうなどと、まるで意味がないではないか。ファミリーレストランに来たうえ、これ見よがしに最も高い料理を注文したとなったら、私の悪評が広まってしまう可能性だってある。

とはいえ、せっかくだから高いものを選んでその味をみてみたいというのも確かである。そうだ、そういうことなら、この店で $ 2 $ 番目に高い料理を注文することにしよう。そう思って料理の金額を書き出してみたが、料理の種類が多いために $ 2 $ 番目に高いものを探すのはなかなか骨が折れる。自分で探すかわりに、プログラムを書いてなんとかできないだろうか？

おっと、プログラムを書き始める前にひとつ言っておくが、最も高い金額の料理が複数あるときには注意してもらいたい。というのは、たとえば $ 4 $ 種類の料理があり、それぞれの金額が $ 100 $ 円、$ 200 $ 円、$ 300 $ 円、$ 300 $ 円であったときには、$ 2 $ 番目に高いものというのは $ 200 $ 円の料理になるということだ。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ : $ A_N $

- $ 1 $ 行目には、料理の種類の個数を表す整数 $ N $ ($ 2\ ≦\ N\ ≦\ 100 $) が与えられる。
- $ 2 $ 行目から $ N $ 行では、それぞれの料理の金額が与えられる。$ N $ 行のうち $ i $ 行目には整数 $ A_i $ ($ 1\ ≦\ A_i\ ≦\ 1,000 $) が書かれており、これは $ i $ 番目の料理の金額が $ A_i $ 円であることを表す。すべての料理の金額が同じであることはない。

## 输出格式

$ N $ 個の料理のうち、$ 2 $ 番目に高いものの金額を $ 1 $ 行に出力せよ。

出力の末尾にも改行をいれること。

## 输入输出样例 #1

### 输入 #1

```
4
100
200
300
300
```

### 输出 #1

```
200
```

## 输入输出样例 #2

### 输入 #2

```
5
50
370
819
433
120
```

### 输出 #2

```
433
```

## 输入输出样例 #3

### 输入 #3

```
6
100
100
100
200
200
200
```

### 输出 #3

```
100
```

## 说明/提示

### Sample Explanation 1

問題文にも出てきた例です。この場合、最も高い料理が $ 300 $ 円で、その次に高い料理は $ 200 $ 円のものになります。