# AT_abc247_b [ABC247B] Unique Nicknames

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc247/tasks/abc247_b

人 $ 1 $, 人 $ 2 $, $ \dots $ 人 $ N $ の $ N $ 人の人がいます。人 $ i $ の姓は $ s_i $、名は $ t_i $ です。

$ N $ 人の人すべてにあだ名をつけることを考えます。人 $ i $ のあだ名 $ a_i $ は以下の条件を満たす必要があります。

- $ a_i $ は人 $ i $ の姓あるいは名と一致する。言い換えると、$ a_i\ =\ s_i $ または $ a_i\ =\ t_i $ の少なくとも一方が成り立つ。
- $ a_i $ は自分以外の人の姓および名のどちらとも一致しない。言い換えると、$ 1\ \leq\ j\ \leq\ N,\ i\ \neq\ j $ を満たすすべての整数 $ j $ について $ a_i\ \neq\ s_j $ かつ $ a_i\ \neq\ t_j $ が成り立つ。

$ N $ 人全員に条件を満たすあだ名をつけることは可能でしょうか。可能ならば `Yes` を、そうでないならば `No` を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ s_1 $ $ t_1 $ $ s_2 $ $ t_2 $ $ \vdots $ $ s_N $ $ t_N $

## 输出格式

$ N $ 人すべてにあだ名をつけることが可能ならば `Yes` を、そうでないならば `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
tanaka taro
tanaka jiro
suzuki hanako
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
3
aaa bbb
xxx aaa
bbb yyy
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
2
tanaka taro
tanaka taro
```

### 输出 #3

```
No
```

## 输入输出样例 #4

### 输入 #4

```
3
takahashi chokudai
aoki kensho
snu ke
```

### 输出 #4

```
Yes
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 100 $
- $ N $ は整数である。
- $ s_i,t_i $ は英小文字からなる $ 1 $ 文字以上 $ 10 $ 文字以下の文字列である。

### Sample Explanation 1

$ a_1\ = $ `taro`, $ a_2\ = $ `jiro`, $ a_3\ = $ `hanako` とすれば、これは問題文にあるあだ名の条件を満たしています。($ a_3 $ は `suzuki` でもよいです。) ここで、$ a_1\ = $ `tanaka` とはできないことに注意してください。なぜならば 人 $ 2 $ の姓 $ s_2 $ もまた `tanaka` であるため、あだ名の条件の $ 2 $ つ目を満たさなくなるからです。

### Sample Explanation 2

問題文の条件を満たすあだ名のつけ方は存在しません。

### Sample Explanation 3

同姓同名である人の組が存在する場合もあります。

### Sample Explanation 4

$ a_1\ = $ `chokudai`, $ a_2\ = $ `kensho`, $ a_3\ = $ `ke` とすればよいです。