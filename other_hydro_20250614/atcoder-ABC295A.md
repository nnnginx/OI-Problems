## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc295/tasks/abc295_a

英小文字からなる $ N $ 個の文字列 $ W_1,W_2,\dots,W_N $ が与えられます。  
 これらのうち一つ以上が `and`, `not`, `that`, `the`, `you` のいずれかと一致するなら `Yes` 、そうでないなら `No` と出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ W_1 $ $ W_2 $ $ \dots $ $ W_N $

## 输出格式
答えを出力せよ。

## 题目大意
由小写字母组成 $N$ 个字符串 $W_1,W_2,...,W_N$。

如果其中有一个或多个是 `and`，`not`，`that`，`the`，`you` 其中之一，就输出 `Yes`，否则就输出 `No`。

```input1
10
in that case you should print yes and not no
```

```output1
Yes
```

```input2
10
in diesem fall sollten sie no und nicht yes ausgeben
```

```output2
No
```

## 提示
### 制約

- $ N $ は $ 1 $ 以上 $ 100 $ 以下の整数
- $ 1\ \le\ |W_i|\ \le\ 50 $ ( $ |W_i| $ は文字列 $ W_i $ の長さ )
- $ W_i $ は英小文字からなる
 
### Sample Explanation 1

例えば $ W_4= $ `you` なので、 `Yes` と出力します。

### Sample Explanation 2

文字列 $ W_i $ はいずれも、 `and`, `not`, `that`, `the`, `you` のいずれとも一致しません。

