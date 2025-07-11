# AT_abc007_2 [ABC007B] 辞書式順序

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc007/tasks/abc007_2

文字列 $ A $ が与えられる。小文字アルファベット(a-z)のみを使って辞書順比較したとき文字列 $ A $ より小さいものを1つ何でも良いので出力せよ。ただし、文字列は $ 1 $ 文字以上 $ 100 $ 文字以下でなければならない。もし存在しない場合は "-1" を出力せよ。

ただし、ある文字列 $ S=S_1S_2...S_n $ と $ T=T_1T_2...T_m $ について、辞書順比較した際に $ S＜T $ であるとは、次のどちらか一方の状態が成り立っていることを言う。

- ある整数 $ i\ (1≦i≦{\rm\ min}(n,m)) $ に関して、 $ 1≦j≦i−1 $ を満たすどの整数 $ j $ に関しても $ S_j=T_j $ が成立し、かつ $ S_i＜T_i $ が成立する
- 任意の整数 $ i\ (1≦i≦{\rm\ min}(n,m)) $ に関して、 常に $ S_i=T_i $ が成立し、かつ $ |S|＜|T| $ である。ただし $ |X| $ は文字列 $ X $ の長さを表すものとする。

なにやら頭が痛くなる記述だが、言い換えると次の通りである。

- それぞれの文字列の同じ位置同士を先頭から比較していって、初めて不一致になったら、その文字同士の(アルファベットでの)比較結果が文字列の全体の比較結果である。 例えば、$ "abcd" $ と $ "ax" $ を比較すると、$ 2 $ 文字目で、$ 'b'\ となるので、"abcd"\ である。 $
- もし、比較している途中で片方の文字列が尽きてしまったら、文字列の長さが短い方が小さい。例えば $ "ab"\ である。 $

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $

- $ 1 $ 行目には、文字列 $ A\ (1\ ≦\ |A|\ ≦\ 11) $ が与えられる。$ |A| $は文字列 $ |A| $ の長さを表す。Aは小文字アルファベット(a-z)のみから成る。

## 输出格式

文字列 $ A $ より小さい文字列を $ 1 $ つ $ 1 $ 行に出力せよ。ただし、小文字アルファベット(a-z)のみを用いており、長さは1以上100以下でなければならない。解が複数ある場合はどれを出力しても良い。存在しない場合は、代わりに "-1" を出力すること。出力の末尾に改行をいれること。

## 输入输出样例 #1

### 输入 #1

```
xyz
```

### 输出 #1

```
xy
```

## 输入输出样例 #2

### 输入 #2

```
c
```

### 输出 #2

```
b
```

## 输入输出样例 #3

### 输入 #3

```
a
```

### 输出 #3

```
-1
```

## 输入输出样例 #4

### 输入 #4

```
aaaaa
```

### 输出 #4

```
aaaa
```

## 说明/提示

### Sample Explanation 1

もちろん、"xy" の他に、"abcd" 等を出力しても正答として扱われる。

### Sample Explanation 2

"a" もしくは "b" が正答として扱われる。

### Sample Explanation 3

"a" より小さい文字列は存在しない。出力する文字列は長さ1以上でなければならないため、""(空文字列)は不適切であることに注意せよ。