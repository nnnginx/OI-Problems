## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc162/tasks/abc162_a

$ 3 $ 桁の整数 $ N $ が与えられます。$ N $ のいずれかの桁に数字の $ 7 $ は含まれますか？

含まれるなら `Yes` を、含まれないなら `No` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
$ N $ のいずれかの桁に $ 7 $ が含まれるなら `Yes` を、含まれないなら `No` を出力せよ。

## 题目大意
读入一个3位的字符串。若这个字符串里有“7”则输出`Yes`，不然输出`No`。

```input1
117
```

```output1
Yes
```

```input2
123
```

```output2
No
```

```input3
777
```

```output3
Yes
```

## 提示
### 制約

- $ 100\ \leq\ N\ \leq\ 999 $

### Sample Explanation 1

$ 117 $ は $ 1 $ の位が $ 7 $ です。

### Sample Explanation 2

$ 123 $ は $ 7 $ を含みません。

