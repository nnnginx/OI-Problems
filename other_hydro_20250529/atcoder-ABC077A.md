## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc077/tasks/abc077_a

縦 $ 2 $ マス、横 $ 3 $ マスのマス目が与えられます。上から $ i $ 行目、左から $ j $ 行目のマスの色は、$ C_{ij} $ で表されます。

このマス目を $ 180 $ 度回転させたとき、元のマス目と一致するなら `YES` を、そうでないなら `NO` を出力するプログラムを作成してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ C_{11}C_{12}C_{13} $ $ C_{21}C_{22}C_{23} $

## 输出格式
マス目を $ 180 $ 度回転させたとき、元のマス目と一致するなら `YES` を、そうでないなら `NO` を出力せよ。

## 题目大意
## 题目描述

给定两个长度为 $3$ 的字符串，如果一个字符串反转后与另一个相等，那么输出 `YES`，否则输出 `NO`。

提示：输出的末尾要输出一个换行符。

## 输入格式：
$C_{1,1},C_{1,2},C_{1,3}$  
$C_{2,1},C_{2,2},C_{2,3}$ 

## 输出格式：

按要求输出 `YES` 或 `NO`。

## 数据范围

输入数据中只会出现两个长度为 $3$ 的，由小写字母组成的字符串。

感谢@福州周圣力  提供的翻译

```input1
pot
top
```

```output1
YES
```

```input2
tab
bet
```

```output2
NO
```

```input3
eye
eel
```

```output3
NO
```

## 提示
### 制約

- $ C_{ij}(1\ \leq\ i\ \leq\ 2,\ 1\ \leq\ j\ \leq\ 3) $ は英小文字である。

### Sample Explanation 1

マス目を $ 180 $ 度回転させると、元のマス目と一致します。

### Sample Explanation 2

マス目を $ 180 $ 度回転させても、元のマス目と一致しません。

