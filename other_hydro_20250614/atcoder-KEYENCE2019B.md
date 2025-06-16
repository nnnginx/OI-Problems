## 题目描述
[problemUrl]: https://atcoder.jp/contests/keyence2019/tasks/keyence2019_b

連続した部分文字列 (空でも良い) を $ 1 $ 度だけ取り除くことで `keyence` に変換することができる文字列をキーエンス型文字列と呼ぶことにします．

英小文字のみから成る文字列 $ S $ が与えられるので，$ S $ がキーエンス型文字列かどうか判定してください．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ S $

## 输出格式
$ S $ がキーエンス型文字列なら `YES` を，そうでないなら `NO` を出力せよ．

## 题目大意
有一个字符串被称为“KEYENCE”字符串，如果它只需删除一次相邻的子字符串（有可能是空的，即不用删除）就可以更改为“KEYENCE”字符串。

给定一个由小写英文字母组成的字符串S，判断字符串S是否是keynce字符串.
如果字符串S是keynce字符串，则输出“YES”；否则，输出“NO”。（记得最后换行！）.

数据范围：S的长度大于等于7并且小于100.
       S是由小写字符组成.

注：keyence是key of science的缩写.（即keyence和keyofscience都可以）

```input1
keyofscience
```

```output1
YES
```

```input2
mpyszsbznf
```

```output2
NO
```

```input3
ashlfyha
```

```output3
NO
```

```input4
keyence
```

```output4
YES
```

## 提示
### 制約

- $ S $ の長さは $ 7 $ 以上 $ 100 $ 以下
- $ S $ は英小文字のみから成る

### Sample Explanation 1

`keyence` とは `key of science` の略です．

