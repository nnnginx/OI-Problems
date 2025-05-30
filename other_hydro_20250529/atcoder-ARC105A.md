## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc105/tasks/arc105_a

すぬけ君は美味しさが $ A,\ B,\ C,\ D $ であるような $ 4 $ 枚のクッキーを持っています。 すぬけ君は $ 1 $ 枚以上のクッキーを選んで食べます。食べるクッキーの美味しさの総和と、残るクッキーの美味しさの総和が等しくなることはありますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ D $

## 输出格式
すぬけ君が食べるクッキーの美味しさの総和と、残るクッキーの美味しさの総和が等しくなることがあるなら `Yes`、そうでなければ `No` を出力せよ。

## 题目大意
## AT_arc105_a Fourtune Cookies 题目翻译

### 题目描述：
你有四块曲奇，每块曲奇都有一个美味程度。

问：**已经吃掉**的曲奇的美味程度总和 和 **还没吃**的曲奇的美味程度总和有没有**相等的时候**？

### 输入格式：
输入以以下形式由标准输入给出:
A B C D
表示四块曲奇的好吃程度

### 输出格式：
如果你已经吃掉的曲奇的美味程度总和和还没吃的曲奇的美味程度总和有相等的时候的话，就输出“是”，否则输出“否”。

### 说明/提示：
#### 制约：
A、B、C、D均为整数且1 ≤ A,B,C,D ≤ 10^8
#### 样例解释1：
你吃掉美味程度为1,4的曲奇的时候，已经吃掉的曲奇的美味的总和和还没吃的曲奇的美味程度的总和相等。
#### 样例解释2：
不管怎么做，已经吃掉的曲奇的美味的总和和还没吃的曲奇的美味程度的总和都不会相等。

```input1
1 3 2 4
```

```output1
Yes
```

```input2
1 2 4 8
```

```output2
No
```

## 提示
### 制約

- 与えられる入力は全て整数
- $ 1\ \leq\ A,B,C,D\ \leq\ 10^{8} $

### Sample Explanation 1

\- すぬけ君が美味しさ $ 1,4 $ のクッキーを食べるとき、食べるクッキーの美味しさの総和と、残るクッキーの美味しさの総和が等しくなります。

### Sample Explanation 2

\- どのようにしても食べるクッキーの美味しさの総和と、残るクッキーの美味しさの総和が等しくなることはありません。

