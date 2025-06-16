## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc180/tasks/abc180_b

$ N $ 次元空間内の点 $ (x_1,\ldots,x_N) $ が与えられます。

原点からこの点までの、マンハッタン距離、ユークリッド距離、チェビシェフ距離をそれぞれ求めてください。 ただし、それぞれの距離は次のように計算されます。

- マンハッタン距離： $ |x_1|+\ldots+|x_N| $
- ユークリッド距離： $ \sqrt{|x_1|^2+\ldots+|x_N|^2} $
- チェビシェフ距離： $ \max(|x_1|,\ldots,|x_N|) $

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ x_1 $ $ \ldots $ $ x_N $

## 输出格式
原点から与えられた点までの、マンハッタン距離、ユークリッド距離、チェビシェフ距離をそれぞれこの順に改行区切りで出力せよ。 正しい値との絶対誤差または相対誤差が $ 10^{-9} $ 以下であれば正解とみなされる。

## 题目大意
给定一个数组，求出三个数：

1、$\lvert x_1 \rvert + \lvert x_2 \rvert + ... + \lvert x_n \rvert$

2、$\sqrt{\lvert x_1 \rvert^2 + \lvert x_2 \rvert^2 + ... + \lvert x_n \rvert^2}$

3、$max (\lvert x_1 \rvert , \lvert x_2 \rvert , ... , \lvert x_n \rvert)$

允许有不大于 $10^{-5}$ 的误差。

translate by [ChrisWangZi](https://www.luogu.com.cn/user/637180)

```input1
2
2 -1
```

```output1
3
2.236067977499790
2
```

```input2
10
3 -1 -4 1 -5 9 2 -6 5 -3
```

```output2
39
14.387494569938159
9
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ -10^5\ \leq\ x_i\ \leq\ 10^5 $
- 入力は全て整数

### Sample Explanation 1

それぞれ次のように計算されます。 - マンハッタン距離： $ |2|+|-1|=3 $ - ユークリッド距離： $ \sqrt{|2|^2+|-1|^2}=2.236067977499789696\ldots $ - チェビシェフ距離： $ \max(|2|,|-1|)=2 $

