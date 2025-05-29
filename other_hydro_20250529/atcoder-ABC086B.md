## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc086/tasks/abc086_b

シカのAtCoDeerくんは二つの正整数 $ a,b $ を見つけました。 $ a $ と $ b $ をこの順につなげて読んだものが平方数かどうか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $

## 输出格式
$ a $ と $ b $ をこの順につなげて読んだものが平方数なら `Yes` を、 そうでないなら `No` を出力せよ。

## 题目大意
将给出的两个正整数a，b连在一起（ab），判断是否为完全平方数 



```input1
1 21
```

```output1
Yes
```

```input2
100 100
```

```output2
No
```

```input3
12 10
```

```output3
No
```

## 提示
### 制約

- $ 1 $ $ <\ = $ $ a,b $ $ <\ = $ $ 100 $
- $ a,b $ は整数

### Sample Explanation 1

$ 121 $ $ = $ $ 11 $ × $ 11 $ なので、平方数です。

### Sample Explanation 2

$ 100100 $ は平方数ではありません。

