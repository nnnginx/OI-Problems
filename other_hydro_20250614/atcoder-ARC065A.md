## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc049/tasks/arc065_a

英小文字からなる文字列 $ S $ が与えられます。 $ T $が空文字列である状態から始め、以下の操作を好きな回数繰り返すことで $ S\ =\ T $ とすることができるか判定してください。

- $ T $ の末尾に `dream` `dreamer` `erase` `eraser` のいずれかを追加する。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S\ =\ T $ とすることができる場合 `YES` を、そうでない場合 `NO` を出力せよ。

## 题目大意
# 题目大意
输入一个以英文小写字母组成的字符串S，规定一个空的字符串T，现在你可对字符串T进行你喜欢的操作，问是否能让字符串T变为字符串S？

**喜欢的操作如下 ：**

在字符串T的末尾加入
“dream”或“dreamer”或“erase”或“eraser”。

------------
## 输入格式
一个字符串S
## 输出格式
若可以输出**YES**,否则输出**NO**。

```input1
erasedream
```

```output1
YES
```

```input2
dreameraser
```

```output2
YES
```

```input3
dreamerer
```

```output3
NO
```

## 提示
### 制約

- $ 1≦|S|≦10^5 $
- $ S $ は英小文字からなる。

### Sample Explanation 1

`erase` `dream` の順で $ T $ の末尾に追加することで $ S\ =\ T $ とすることができます。

### Sample Explanation 2

`dream` `eraser` の順で $ T $ の末尾に追加することで $ S\ =\ T $ とすることができます。

