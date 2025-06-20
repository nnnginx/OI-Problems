# AT_xmascon18_j Japanese Exponentation

## 题目描述

[problemUrl]: https://atcoder.jp/contests/xmascon18/tasks/xmascon18_j

漢数字で表される非負整数に対する，演算「$ a $ の $ b $ 乗」のみからなる式 $ S $ が与えられるので，その値を十億九で割った余りを漢数字で出力せよ．

非負整数は漢数字によって，標準的な日本語で表記する．以下の点に注意せよ．

- 本問で用いられる文字は `〇`, `一`, `二`, `三`, `四`, `五`, `六`, `七`, `八`, `九`, `十`, `百`, `千`, `万`, `億` である．
- $ 0 $ は「〇」である．正の整数には文字 `〇` は用いない．
- $ 10^3 $ は「千」である (「一千」ではない)．同様に，$ 10^7 $ は「千万」，$ 10^{11} $ は「千億」である．
- $ 10^4 $ は「一万」である (「万」ではない)．同様に，$ 10^8 $ は「一億」である．

また，「〇の〇乗」は一であると約束する．

## 输入格式

> $ S $

入力の文字コードは UTF-8 (BOM なし) である．`六` は U+516D である (互換文字の U+F9D1 ではない)．

## 输出格式

式 $ S $ の計算結果を十億九で割った余りを漢数字で出力せよ．出力の文字コードは UTF-8 (BOM なし) であること．`六` は U+516D であること．

## 输入输出样例 #1

### 输入 #1

```
四の三の二乗乗
```

### 输出 #1

```
二十六万二千百四十四
```

## 输入输出样例 #2

### 输入 #2

```
四の三乗の二乗
```

### 输出 #2

```
四千九十六
```

## 输入输出样例 #3

### 输入 #3

```
十億十
```

### 输出 #3

```
一
```

## 输入输出样例 #4

### 输入 #4

```
一億二千三百四十五万六千七百八十九の二の〇の〇乗乗乗
```

### 输出 #4

```
六億千三百一万六千三百十九
```

## 说明/提示

### 制約

- $ S $ に含まれる文字の個数は一以上十万以下である．
- $ S $ の各文字は `〇`, `一`, `二`, `三`, `四`, `五`, `六`, `七`, `八`, `九`, `十`, `百`, `千`, `万`, `億`, `の`, `乗` のいずれかである．
- $ S $ は問題文の仕様を満たす正しい式である．

### 部分点

- $ S $ に含まれる文字の個数が千以下であるデータセットに正解した場合は，二十点が与えられる．
- 追加制約のないデータセットに正解した場合は，上記とは別に八十点が与えられる．

### Sample Explanation 4

サンプル入出力ファイルは\[こちら\](https://img.atcoder.jp/xmascon18/japanese-sample.zip)からダウンロードできる．