# AT_abc344_a [ABC344A] Spoiler

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc344/tasks/abc344_a

英小文字と `|` のみからなる文字列 $ S $ が与えられます。$ S $ は `|` をちょうど $ 2 $ 個含むことが保証されます。

$ 2 $ つの `|` の間にある文字および `|` を $ S $ から削除した文字列を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
atcoder|beginner|contest
```

### 输出 #1

```
atcodercontest
```

## 输入输出样例 #2

### 输入 #2

```
|spoiler|
```

### 输出 #2

```

```

## 输入输出样例 #3

### 输入 #3

```
||xyz
```

### 输出 #3

```
xyz
```

## 说明/提示

### 制約

- $ S $ は英小文字および `|` のみからなる長さ $ 2 $ 以上 $ 100 $ 以下の文字列
- $ S $ は `|` をちょうど $ 2 $ 個含む
 
### Sample Explanation 1

$ 2 $ つの `|` に挟まれた文字を全て削除して出力してください。

### Sample Explanation 2

全ての文字が削除されることもあります。