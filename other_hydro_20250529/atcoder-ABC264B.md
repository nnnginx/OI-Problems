## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc264/tasks/abc264_b

次の図に示す、各マスが黒または白に塗られた縦 $ 15 $ 行 $ \times $ 横 $ 15 $ 列のグリッドにおいて、 上から $ R $ 行目、左から $ C $ 列目のマスが何色かを出力して下さい。

![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc264_b/1d08398813abcc960441841276a0737d88e46e2f.png)

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ R $ $ C $

## 输出格式
図のグリッドにおいて上から $ R $ 行目、左から $ C $ 列目のマスが黒色の場合は `black` と、白色の場合は `white` と出力せよ。 ジャッジは英小文字と英大文字を厳密に区別することに注意せよ。

## 题目大意
输入一个 $R$ 一个 $C$，问题目描述中图片的第 $R$ 行第 $C$ 列是黑是白？黑输出 $\tt black$，白输出 $\tt white$。

```input1
3 5
```

```output1
black
```

```input2
4 5
```

```output2
white
```

## 提示
### 制約

- $ 1\ \leq\ R,\ C\ \leq\ 15 $
- $ R,\ C $ は整数

### Sample Explanation 1

図のグリッドにおいて上から $ 3 $ 行目、左から $ 5 $ 列目のマスは黒色です。 よって、`black` と出力します。

### Sample Explanation 2

図のグリッドにおいて上から $ 4 $ 行目、左から $ 5 $ 列目のマスは白色です。 よって、`white` と出力します。

