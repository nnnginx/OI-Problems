# AT_tdpc_iwi イウィ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tdpc/tasks/tdpc_iwi

入力は以下の形式で標準入力から与えられる。

> $ s $

 答えを一行に出力せよ。 ```

iwiwii
```

```

2
```

```

iwiwwwiiiwiwiwiiwii
```

```

5
```

## 输入格式

无

## 输出格式

无

## 说明/提示

### Constraints

 $ s $ は i と w からなる文字列である。すぬけ君は、この中から連続する三文字が "iwi" となっている部分を取り除く操作を繰り返すことができる。(iwi を取り除くと、その左側と右側にあった文字列が連結され、長さが三文字短い新しい文字列ができる。) 操作を行うことのできる回数の最大値を求めよ。

- - - - - -

- $ 1\ <\ =\ |s|\ <\ =\ 300 $
- Each character in $ s $ will be either 'i' or 'w'.