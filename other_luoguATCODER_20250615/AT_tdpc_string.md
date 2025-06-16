# AT_tdpc_string 文字列

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tdpc/tasks/tdpc_string

入力は以下の形式で標準入力から与えられる。

> $ freq_1 $ $ ... $ $ freq_{26} $

 答えを一行に出力せよ。 ```

1 0 2 1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
```

```

6
```

```

1 1 1 1 1 1 1 1 1 1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
```

```

3628800
```

## 输入格式

无

## 输出格式

无

## 说明/提示

### Constraints

 以下の条件を満たす文字列の個数を mod 1,000,000,007 で求めよ。

- a を $ freq_1 $ 個、b を $ freq_2 $ 個、... z を $ freq_{26} $ 個含む (他の文字は含まない)。
- 同じ文字が隣り合うことはない。

- - - - - -

- $ 0\ <\ =\ freq_i\ <\ =\ 10 $
- At least one of $ freq_i $ will be nonzero.