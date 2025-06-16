## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc066/tasks/abc066_b

同じ文字列を $ 2 $ つ並べてできる文字列のことを偶文字列と呼ぶことにします。 例えば、 `xyzxyz` や `aaaaaa` は偶文字列ですが、`ababab` や `xyzxy` は偶文字列ではありません。

アルファベットの小文字からなる偶文字列 $ S $ が与えられます。 $ S $ の末尾の文字を $ 1 $ 文字以上消して作れる偶文字列のうち、最も長い偶文字列の長さを求めて下さい。 与えられる入力では、条件を満たす $ 1 $ 文字以上の文字列が存在することが保証されています。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えとなる文字列の長さを出力せよ。

## 题目大意
如果某个串可以由两个一样的串前后连接得到，我们就称之为“偶串”。比如说“xyzxyz”和“aaaaaa”是偶串，而“ababab”和“xyzxy”则不是偶串。

输入一个字符串S，查找可以通过从S的末尾删除一个或多个字符获得的最长偶数字符串的长度。确保给定输入存在这样的非空字符串。

输出这个非空字符串的长度

```input1
abaababaab
```

```output1
6
```

```input2
xxxx
```

```output2
2
```

```input3
abcabcabcabc
```

```output3
6
```

```input4
akasakaakasakasakaakas
```

```output4
14
```

## 提示
### 制約

- $ 2\ \leq\ |S|\ \leq\ 200 $
- $ S $ は小文字のアルファベットのみからなる偶文字列である。
- $ S $ に対して、条件を満たす $ 1 $ 文字以上の文字列が存在する。

### Sample Explanation 1

`abaababaab` は偶文字列ですが、 $ 1 $ 文字も消していないので条件を満たしません。 `abaababaa` は偶文字列ではありません。 `abaababa` は偶文字列ではありません。 `abaabab` は偶文字列ではありません。 `abaaba` は偶文字列です。よって、答えは `abaaba` の長さである $ 6 $ です。

### Sample Explanation 2

`xxx` は偶文字列ではありません。 `xx` は偶文字列です。

### Sample Explanation 3

条件を満たす文字列は `abcabc` なので、答えは $ 6 $ です。

### Sample Explanation 4

条件を満たす文字列は `akasakaakasaka` なので、答えは $ 14 $ です。

