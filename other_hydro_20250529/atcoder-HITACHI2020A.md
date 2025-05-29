## 题目描述
[problemUrl]: https://atcoder.jp/contests/hitachi2020/tasks/hitachi2020_a

文字列 `hi` が $ 1 $ 個以上繋がってできる文字列を、 hitachi文字列 と定義します。

例えば、 `hi` や `hihi` などは hitachi文字列 であり、 `ha` や `hii` は hitachi文字列 ではありません。

文字列 $ S $ が与えられるので、 $ S $ が hitachi文字列 かどうかを判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S $ が hitachi文字列 であれば `Yes` を、そうでなければ `No` を出力せよ。

## 题目大意
输入一个长度不大于 $10$ 的，完全由英文小写字母组成的字符串 $s$，请判断 $s$ 是否是由一个或多个`hi`连接而成的字符串。

```input1
hihi
```

```output1
Yes
```

```input2
hi
```

```output2
Yes
```

```input3
ha
```

```output3
No
```

## 提示
### 制約

- $ S $ の長さは $ 1 $ 以上 $ 10 $ 以下
- $ S $ は英小文字列

### Sample Explanation 1

`hihi` は `hi` を $ 2 $ 個繋げてできる文字列なので、 hitachi文字列です。

