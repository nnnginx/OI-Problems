## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc082/tasks/abc082_b

英小文字のみからなる文字列 $ s $, $ t $ が与えられます。 あなたは、$ s $ の文字を好きな順に並べ替え、文字列 $ s' $ を作ります。 また、$ t $ の文字を好きな順に並べ替え、文字列 $ t' $ を作ります。 このとき、辞書順で $ s'\ <\ t' $ となるようにできるか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ s $ $ t $

## 输出格式
辞書順で $ s'\ <\ t' $ となるようにできるならば `Yes` を、できないならば `No` を出力せよ。

## 题目大意
给定$2$个字串（$\color{blue}\text{长度<100}\color{red}\text{可能有空格}$），判断是否可以通过排序这$2$个串使得$\color{purple}\text{第一个串<第二个串}\color{red}\text{(指的是字典序!)}$

```input1
yx
axy
```

```output1
Yes
```

```input2
ratcode
atlas
```

```output2
Yes
```

```input3
cd
abc
```

```output3
No
```

```input4
w
ww
```

```output4
Yes
```

```input5
zzz
zzz
```

```output5
No
```

## 提示
### 注釈

長さ $ N $ の文字列 $ a\ =\ a_1\ a_2\ ...\ a_N $ および長さ $ M $ の文字列 $ b\ =\ b_1\ b_2\ ...\ b_M $ について、辞書順で $ a\ <\ b $ であるとは、次の $ 2 $ つの条件のいずれかが成り立つことをいう;

- $ N\ <\ M $ かつ $ a_1\ =\ b_1 $, $ a_2\ =\ b_2 $, ..., $ a_N\ =\ b_N $ である。
- ある $ i $ ($ 1\ \leq\ i\ \leq\ N,\ M $) が存在して、$ a_1\ =\ b_1 $, $ a_2\ =\ b_2 $, ..., $ a_{i\ -\ 1}\ =\ b_{i\ -\ 1} $ かつ $ a_i\ <\ b_i $ である。 ただし、文字どうしはアルファベット順で比較される。

例えば、`xy` $ < $ `xya` であり、`atcoder` $ < $ `atlas` である。

### 制約

- $ s $, $ t $ の長さは $ 1 $ 以上 $ 100 $ 以下である。
- $ s $, $ t $ は英小文字のみからなる。

### Sample Explanation 1

例えば、`yx` を `xy` と並べ替え、`axy` を `yxa` と並べ替えれば、`xy` $ < $ `yxa` となります。

### Sample Explanation 2

例えば、`ratcode` を `acdeort` と並べ替え、`atlas` を `tslaa` と並べ替えれば、`acdeort` $ < $ `tslaa` となります。

### Sample Explanation 3

`cd`, `abc` をそれぞれどのように並べ替えても、目標を達成できません。

