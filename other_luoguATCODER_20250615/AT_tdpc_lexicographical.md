# AT_tdpc_lexicographical 辞書順

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tdpc/tasks/tdpc_lexicographical

入力は以下の形式で標準入力から与えられる。

> $ s $ $ K $

 答えを一行に出力せよ。 ```

eel
6
```

```

Eel
```

```

lexicographical
100
```

```

capal
```

## 输入格式

无

## 输出格式

无

## 说明/提示

### Constraints

 文字列 $ s $ の空でない部分列のうち、辞書順で $ K $ 番目のものを求めよ。そのようなものが存在しない場合は "Eel" (quotes for clarity) と出力せよ。   
 ただし、$ s $ から何文字か取り除き (0 文字でもよい)、残りの文字を順番を変えずにつなげたものを部分列という。たとえば、"aba" の部分列は "a", "b", "aa", "ab", "ba", "aba" の 6 個である。"a" は異なる場所に二回現れるが、文字列として同じであれば区別しないものとする。

- - - - - -

- $ 1\ <\ =\ |s|\ <\ =\ 1000000 $
- Each character in s will be a lowercase letter ('a'-'z').
- $ 1\ <\ =\ K\ <\ =\ 10^{18} $