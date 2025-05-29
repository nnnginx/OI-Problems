## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc062/tasks/arc074_a

縦 $ H $ ブロック、横 $ W $ ブロックの板チョコがあります。 すぬけ君は、この板チョコをちょうど $ 3 $ つのピースに分割しようとしています。 ただし、各ピースはブロックの境目に沿った長方形でなければなりません。

すぬけ君は、$ 3 $ つのピースの面積 (ブロック数) をできるだけ均等にしようとしています。 具体的には、$ 3 $ つのピースの面積の最大値を $ S_{max} $、最小値を $ S_{min} $ としたとき、$ S_{max}\ -\ S_{min} $ を最小化しようとしています。 $ S_{max}\ -\ S_{min} $ の最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $

## 输出格式
$ S_{max}\ -\ S_{min} $ の最小値を出力せよ。

## 题目大意
给定一个大小为 $H \times W$ 的矩形，由 $H \times W$ 个小矩形组成。

你需要将这个大矩形切成三个部分，要求只能沿着小矩形的边切且且出来的三个部分必须均为矩形。

请最小化切出来的三个矩形中最大矩形与最小矩形的差，并输出这个差值。

```input1
3 5
```

```output1
0
```

```input2
4 5
```

```output2
2
```

```input3
5 5
```

```output3
4
```

```input4
100000 2
```

```output4
1
```

```input5
100000 100000
```

```output5
50000
```

## 提示
### 制約

- $ 2\ <\ =\ H,\ W\ <\ =\ 10^5 $

### Sample Explanation 1

次図のように分割すると、$ S_{max}\ -\ S_{min}\ =\ 5\ -\ 5\ =\ 0 $ となります。 !\[2a9b2ef47b750c0b7ba3e865d4fb4203.png\](https://atcoder.jp/img/arc074/2a9b2ef47b750c0b7ba3e865d4fb4203.png)

### Sample Explanation 2

次図のように分割すると、$ S_{max}\ -\ S_{min}\ =\ 8\ -\ 6\ =\ 2 $ となります。 !\[a42aae7aaaadc4640ac5cdf88684d913.png\](https://atcoder.jp/img/arc074/a42aae7aaaadc4640ac5cdf88684d913.png)

### Sample Explanation 3

次図のように分割すると、$ S_{max}\ -\ S_{min}\ =\ 10\ -\ 6\ =\ 4 $ となります。 !\[eb0ad0cb3185b7ae418e21c472ff7f26.png\](https://atcoder.jp/img/arc074/eb0ad0cb3185b7ae418e21c472ff7f26.png)

