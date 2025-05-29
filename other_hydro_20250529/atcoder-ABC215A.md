## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc215/tasks/abc215_a

文字列 $ S $ が与えられるので、この文字列が `Hello,World!` と完全に一致するなら `AC` 、そうでないなら `WA` と出力してください。

 「完全に一致する」とは？文字列 $ A $ と $ B $ が完全に一致するとは、文字列 $ A $ と $ B $ の長さが等しく、かつ全ての $ 1\ \le\ i\ \le\ |A| $ を満たす整数 $ i $ について $ A $ の先頭から $ i $ 文字目と $ B $ の先頭から $ i $ 文字目とが(英大文字か小文字かも含めて)一致することを指します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを出力せよ。

## 题目大意
输入一个仅由英文大小写字母以及逗号和叹号（均为半角字符）组成的字符串 $s$ 。判断该字符串是否与 “Hello,World!” **完全一致**，若完全一致输出“AC”，否则输出“WA”。（所有上文中出现的字符串均不包含双引号）

```input1
Hello,World!
```

```output1
AC
```

```input2
Hello,world!
```

```output2
WA
```

```input3
Hello!World!
```

```output3
WA
```

## 提示
### 制約

- $ 1\ \le\ |S|\ \le\ 15 $
- $ S $ は英大小文字, `,`, `!` のみからなる

### Sample Explanation 1

文字列 $ S $ は `Hello,World!` と完全に一致します。

### Sample Explanation 2

先頭から $ 7 $ 文字目の `W` が、 `Hello,World!` では大文字ですが $ S $ では小文字です。よって $ S $ は `Hello,World!` と一致しません。

