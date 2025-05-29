## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc045/tasks/abc045_a

上底の長さが $ a $、下底の長さが $ b $、高さが $ h $ の台形があります。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc045_a/695fd302082c8c27a3f1814f7489c8be1c4f74c9.png)台形の例

 

この台形の面積を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $ $ h $

## 输出格式
台形の面積を整数で出力せよ。面積が整数になることは保障されている。

## 题目大意
一个梯形，给出上底a，下底b，高h的长度，求它的面积~~~

```input1
3
4
2
```

```output1
7
```

```input2
4
4
4
```

```output2
16
```

## 提示
### 制約

- $ 1\ \leq\ a\ \leq\ 100 $
- $ 1\ \leq\ b\ \leq\ 100 $
- $ 1\ \leq\ h\ \leq\ 100 $
- 入力で与えられる値はすべて整数
- $ h $ は偶数

### Sample Explanation 1

上底の長さ $ 3 $、下底の長さ $ 4 $、高さ $ 2 $ の台形の面積は、 $ (3+4)×2/2\ =\ 7 $ です。

### Sample Explanation 2

この例で与えられるのは平行四辺形ですが、平行四辺形も台形です。

