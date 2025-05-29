## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc093/tasks/abc093_a

`a`,`b`,`c` からなる長さ $ 3 $ の文字列 $ S $ が与えられます。$ S $ を `abc` を並び替えて作ることができるかどうか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S $ を `abc` を並び替えて作ることができるなら `Yes` を、そうでないなら `No` を出力せよ。

## 题目大意
给你一个字符串$S$

$S$由$a,b,c$三种字符组成

问是否可以通过重排使得$S=abc$

$|S|=3$

```input1
bac
```

```output1
Yes
```

```input2
bab
```

```output2
No
```

```input3
abc
```

```output3
Yes
```

```input4
aaa
```

```output4
No
```

## 提示
### 制約

- $ |S|=3 $
- $ S $ は `a`,`b`,`c` からなる

### Sample Explanation 1

`bac` の $ 1 $ 文字目と $ 2 $ 文字目を入れ替えると `abc` になります。

