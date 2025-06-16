## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc179/tasks/abc179_a

AtCoder 王国では、英小文字を用いる高橋語という言語が使われています。

高橋語では、名詞の複数形は次のルールで綴られます。

- 単数形の末尾が `s` 以外なら、単数形の末尾に `s` をつける
- 単数形の末尾が `s` なら、単数形の末尾に `es` をつける

高橋語の名詞の単数形 $ S $ が与えられるので、複数形を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
与えられた高橋語の複数形を出力せよ。

## 题目大意
在一个王国，有一种语言叫高桥语，这种语言是用英文小写字母组成的。现在输入一个单词，为字符串$s$。

- 如果这个单词的单数形式不是以`s`结尾的，在末尾加上`s`。

- 如果这个单词的单数形式是以`s`结尾的，在末尾加`es`。

保证：1.字符串`s`不超过1000；
2.均为小写字母。

Translated by CodingID

```input1
apple
```

```output1
apples
```

```input2
bus
```

```output2
buses
```

```input3
box
```

```output3
boxs
```

## 提示
### 制約

- $ S $ は長さ $ 1 $ 以上 $ 1000 $ 以下の文字列
- $ S $ は英小文字のみを含む

### Sample Explanation 1

`apple` の末尾は `e` なので、複数形は `apples` になります。

### Sample Explanation 2

`bus` の末尾は `s` なので、複数形は `buses` になります。

