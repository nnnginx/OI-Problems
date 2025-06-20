# AT_abc035_a [ABC035A] テレビ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc035/tasks/abc035_a

高橋君は画面の幅が $ W $ 、高さが $ H $ のテレビを持っています。

このテレビの画面アスペクト比 $ W:H $ が $ 4:3 $ か $ 16:9 $ か判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ W $ $ H $

- $ 1 $ 行目にテレビの画面の幅と高さを表す $ 2 $ つの整数 $ W,H\ (1≦H\ <\ W≦10^5) $ が空白区切りで与えられる。
- テレビの画面アスペクト比は $ 4:3 $ か $ 16:9 $ になることが保証される。

## 输出格式

高橋君のテレビの画面アスペクト比 $ W:H $ が $ 4:3 $ ならば`4:3`を、 $ 16:9 $ ならば `16:9` を $ 1 $ 行に出力せよ。改行を忘れないこと。

## 输入输出样例 #1

### 输入 #1

```
4 3
```

### 输出 #1

```
4:3
```

## 输入输出样例 #2

### 输入 #2

```
16 9
```

### 输出 #2

```
16:9
```

## 输入输出样例 #3

### 输入 #3

```
28 21
```

### 输出 #3

```
4:3
```

## 说明/提示

### Sample Explanation 1

\- 画面の幅が $ 4 $ 、高さが $ 3 $ のテレビの画面アスペクト比は $ 4:3 $ なので`4:3`と出力してください。

### Sample Explanation 2

\- 画面の幅が $ 16 $ 、高さが $ 9 $ のテレビの画面アスペクト比は $ 16:9 $ なので`16:9`と出力してください。