## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc071/tasks/abc071_b

英小文字からなる文字列 $ S $ が与えられます． $ S $ に現れない英小文字であって，最も辞書順（アルファベット順）で小さいものを求めてください． ただし，$ S $ にすべての英小文字が現れる場合は，代わりに `None` を出力してください．

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S $ に現れない英小文字であって，最も辞書順で小さいものを出力せよ． ただし，$ S $ にすべての英小文字が現れる場合は，代わりに `None` を出力せよ．

## 题目大意
给出由小写字母组成的字符串$S$。 查找未出现在$S$中且字母顺序最小的小写字母。如果所有小写字母都出现在$S$中，则输出"None"。

```input1
atcoderregularcontest
```

```output1
b
```

```input2
abcdefghijklmnopqrstuvwxyz
```

```output2
None
```

```input3
fajsonlslfepbjtsaayxbymeskptcumtwrmkkinjxnnucagfrg
```

```output3
d
```

## 提示
### 制約

- $ 1\ \leq\ |S|\ \leq\ 10^5 $ ($ |S| $ は文字列 $ S $ の長さ)
- $ S $ は英小文字のみからなる．

### Sample Explanation 1

`atcoderregularcontest` という文字列には `a` は現れますが `b` は現れません．

### Sample Explanation 2

この文字列には，すべての英小文字が現れます．

