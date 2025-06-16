## 题目描述
[problemUrl]: https://atcoder.jp/contests/cf17-final/tasks/cf17_final_a

文字列 $ S $ が与えられます。

高橋君はこの文字列の好きな位置に好きなだけ文字 `A` を挿入することができます。

$ S $ を `AKIHABARA` に変えることはできるでしょうか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S $ を `AKIHABARA` に変えることができる場合は `YES`、できない場合は `NO` を出力せよ。

## 题目大意
# 题目描述
输入一个字符串S，高桥君在其中任意位置插入A，问是否可以变成AKIHABARA
## 输入格式
一个字符串S
## 输出格式
可以输出YES，否则输出NO

```input1
KIHBR
```

```output1
YES
```

```input2
AKIBAHARA
```

```output2
NO
```

```input3
AAKIAHBAARA
```

```output3
NO
```

## 提示
### 制約

- $ 1\ \leq\ |S|\ \leq\ 50 $
- $ S $ は大文字アルファベットのみからなる。

### Sample Explanation 1

先頭、`H`の直後、`B`の直後、末尾の $ 4 $ 箇所に $ 1 $ つずつ挿入すれば良いです。

### Sample Explanation 2

`AKIHABARA` が正しい綴りです。

