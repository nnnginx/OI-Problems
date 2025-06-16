## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc292/tasks/abc292_a

英小文字のみからなる文字列 $ S $ が与えられます。

$ S $ の各文字を英大文字に変換して得られる文字列 $ T $ を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ T $ を出力せよ。

## 题目大意
- 有一个小写字母序列 $S$。
- 把它转换成大写字母序列后输出。
- $1\le |S|\le 100$。

```input1
abc
```

```output1
ABC
```

```input2
a
```

```output2
A
```

```input3
abcdefghjiklnmoqprstvuwxyz
```

```output3
ABCDEFGHJIKLNMOQPRSTVUWXYZ
```

## 提示
### 制約

- $ S $ は英小文字のみからなる、長さが $ 1 $ 以上 $ 100 $ 以下の文字列
 
### Sample Explanation 1

`abc` の各文字を英大文字に変換すると `ABC` になります。

