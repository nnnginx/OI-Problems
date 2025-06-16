## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc183/tasks/abc183_a

ReLU関数は以下のように定義されます。 [](ReLU(x)%20=%0D%0A%20%20%20%20%20%20%20%20%5Cbegin%7Bcases%7D%0D%0A%20%20%20%20%20%20%20%20%20%20%20%20x%20&%20(x%20%5Cgeqq%200)%20%5C%0D%0A%20%20%20%20%20%20%20%20%20%20%20%200%20&%20(x%20<%200)%20%5C%0D%0A%20%20%20%20%20%20%20%20%5Cend%7Bcases%7D)

![図](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc183_a/e2acda65afcd665d28e66512dfcd8da2f90d6ee9.png)

整数 $ x $ が与えられるので $ ReLU(x) $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ x $

## 输出格式
答えを整数で出力せよ。

## 题目大意
输入一个整数 $x$，如果 $x\ge0$ 则输出 $x$，否则输出 $0$。

```input1
1
```

```output1
1
```

```input2
0
```

```output2
0
```

```input3
-1
```

```output3
0
```

## 提示
### 制約

- $ x $ は整数
- $ -10\ \leq\ x\ \leq\ 10 $

### Sample Explanation 1

$ 1\ \geq\ 0 $ なので $ ReLU(1)\ =\ 1 $ です。

