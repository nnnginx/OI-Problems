## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc069/tasks/abc069_b

`internationalization` という英単語は、`i18n` と略されることがあります。 これは、先頭文字 `i` と末尾文字 `n` の間に $ 18 $ 文字が挟まっていることに由来します。

長さ $ 3 $ 以上の英小文字のみからなる文字列 $ s $ が与えられます。 同様の規則によって $ s $ を略してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ s $

## 输出格式
$ s $ を略したものを出力せよ。

## 题目大意
输入一个字符串，将这个字符串的第一个和最后一个字母中间的字母个数替换为数字，再将其输出。

```input1
internationalization
```

```output1
i18n
```

```input2
smiles
```

```output2
s4s
```

```input3
xyz
```

```output3
x1z
```

## 提示
### 制約

- $ 3\ <\ =\ |s|\ <\ =\ 100 $ (ただし、$ |s| $ は $ s $ の長さを表す。)
- $ s $ は英小文字のみからなる。

