## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc164/tasks/abc164_a

羊が $ S $ 匹、狼が $ W $ 匹います。

狼の数が羊の数以上のとき、羊は狼に襲われてしまいます。

羊が狼に襲われるなら `unsafe`、襲われないなら `safe` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $ $ W $

## 输出格式
羊が狼に襲われるなら `unsafe`、襲われないなら `safe` を出力せよ。

## 题目大意
草原上有 $S$ 头羊，$W$ 头狼。如果 羊的数量比狼多，输出 `safe`，否则输出 `unsafe`。

```input1
4 5
```

```output1
unsafe
```

```input2
100 2
```

```output2
safe
```

```input3
10 10
```

```output3
unsafe
```

## 提示
### 制約

- $ 1\ \leq\ S\ \leq\ 100 $
- $ 1\ \leq\ W\ \leq\ 100 $

### Sample Explanation 1

羊が $ 4 $ 匹、狼が $ 5 $ 匹います。狼の数が羊の数以上なので、羊は狼に襲われてしまいます。

### Sample Explanation 2

多勢に無勢です。

