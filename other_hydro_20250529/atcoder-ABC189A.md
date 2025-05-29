## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc189/tasks/abc189_a

あなたはスロットマシーンで遊んでいます。

スロットを回した結果は $ 3 $ 文字の英大文字 $ C_1,C_2,C_3 $ で表され、これらが全て同じ文字であるとき当たりです。

当たりかどうか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ C_1\ C_2\ C_3 $

## 输出格式
当たりなら `Won` を、当たりでないなら `Lost` を出力せよ。

## 题目大意
# 简要题意

给出三个大写字母，判断它们是否相同。

```input1
SSS
```

```output1
Won
```

```input2
WVW
```

```output2
Lost
```

## 提示
### 制約

- $ C_i $ は英大文字

### Sample Explanation 1

全て同じ文字なので当たりです。

### Sample Explanation 2

当たりではありません。

