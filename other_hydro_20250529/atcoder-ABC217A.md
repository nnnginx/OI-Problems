## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc217/tasks/abc217_a

相異なる二つの文字列 $ S,\ T $ が与えられます。  
 $ S $ が $ T $ よりも辞書順で小さい場合は `Yes` を、大きい場合は `No` を出力してください。

 辞書順とは？ 辞書順とは簡単に説明すると「単語が辞書に載っている順番」を意味します。より厳密な説明として、相異なる文字列 $ S $ と文字列 $ T $ の大小を判定するアルゴリズムを以下に説明します。

以下では「 $ S $ の $ i $ 文字目の文字」を $ S_i $ のように表します。また、 $ S $ が $ T $ より辞書順で小さい場合は $ S\ \lt\ T $ 、大きい場合は $ S\ \gt\ T $ と表します。

1. $ S $ と $ T $ のうち長さが短い方の文字列の長さを $ L $ とします。$ i=1,2,\dots,L $ に対して $ S_i $ と $ T_i $ が一致するか調べます。
2. $ S_i\ \neq\ T_i $ である $ i $ が存在する場合、そのような $ i $ のうち最小のものを $ j $ とします。そして、$ S_j $ と $ T_j $ を比較して、 $ S_j $ がアルファベット順で $ T_j $ より小さい場合は $ S\ \lt\ T $ 、大きい場合は $ S\ \gt\ T $ と決定して、アルゴリズムを終了します。
3. $ S_i\ \neq\ T_i $ である $ i $ が存在しない場合、 $ S $ と $ T $ の長さを比較して、$ S $ が $ T $ より短い場合は $ S\ \lt\ T $ 、長い場合は $ S\ \gt\ T $ と決定して、アルゴリズムを終了します。

なお、主要なプログラミング言語の多くでは、文字列の辞書順による比較は標準ライブラリに含まれる関数や演算子として実装されています。詳しくは各言語のリファレンスをご参照ください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $ $ T $

## 输出格式
$ S $ が $ T $ より辞書順で小さい場合は `Yes` を、大きい場合は `No` を出力せよ。

## 题目大意
给出两个不同的完全由英文小写字母组成的字符串 $s,t$ ，问 $s$ 的字典序是否小于 $t$ 。

```input1
abc atcoder
```

```output1
Yes
```

```input2
arc agc
```

```output2
No
```

```input3
a aa
```

```output3
Yes
```

## 提示
### 制約

- $ S,\ T $ は英小文字からなる長さ $ 1 $ 以上 $ 10 $ 以下の相異なる文字列である。

### Sample Explanation 1

`abc` と `atcoder` は $ 1 $ 文字目が同じで $ 2 $ 文字目が異なります。 アルファベットの `b` は `t` よりもアルファベット順で先に来るので、 `abc` の方が `atcoder` よりも辞書順で小さいことがわかります。

