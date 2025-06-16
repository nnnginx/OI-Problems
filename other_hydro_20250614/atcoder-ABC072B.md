## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc072/tasks/abc072_b

英小文字からなる文字列 $ s $ が与えられます。前から数えて奇数文字目だけ抜き出して作った文字列を出力してください。 ただし、文字列の先頭の文字を1文字目とします。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ s $

## 输出格式
前から数えて奇数文字目だけ抜き出して作った文字列を出力せよ。

## 题目大意
题目：给定一个字符串，输出所有索引号为奇数的位置上的字符。

```input1
atcoder
```

```output1
acdr
```

```input2
aaaa
```

```output2
aa
```

```input3
z
```

```output3
z
```

```input4
fukuokayamaguchi
```

```output4
fkoaaauh
```

## 提示
### 制約

- $ s $ の各文字は英小文字
- $ 1\ <\ =|s|\ <\ =10^5 $

### Sample Explanation 1

$ 1 $ 文字目の `a`, $ 3 $ 文字目の `c`, $ 5 $ 文字目の `d`, $ 7 $ 文字目の `r` を取り出して `acdr` となります。

