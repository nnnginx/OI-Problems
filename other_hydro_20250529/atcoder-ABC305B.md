## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc305/tasks/abc305_b

直線上に $ 7 $ 個の点 $ A,\ B,\ C,\ D,\ E,\ F,\ G $ がこの順に並んでいます。(下の図も参考にしてください)  
 隣り合う点の距離は次の通りです。

- 点 $ A $ と点 $ B $ の距離は $ 3 $
- 点 $ B $ と点 $ C $ の距離は $ 1 $
- 点 $ C $ と点 $ D $ の距離は $ 4 $
- 点 $ D $ と点 $ E $ の距離は $ 1 $
- 点 $ E $ と点 $ F $ の距離は $ 5 $
- 点 $ F $ と点 $ G $ の距離は $ 9 $
 
![image](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc305_b/5b482e7e351ae7c5f6bc500e0b913716b6d7e500.png)

2 つの英大文字 $ p,\ q $ が与えられます。$ p,\ q $ は `A`,`B`,`C`,`D`,`E`,`F`,`G` のいずれかで、 $ p\ \neq\ q $ が成り立ちます。  
 点 $ p $ と点 $ q $ の間の距離を答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ p $ $ q $

## 输出格式
点 $ p $ と点 $ q $ の間の距離を出力せよ。

## 题目大意
数轴上有 $7$ 个点 $A(0),B(3),C(4),D(8),E(9),F(14),G(23)$。

给定**其中两点**，求两点之间的距离。

```input1
A C
```

```output1
4
```

```input2
G B
```

```output2
20
```

```input3
C F
```

```output3
10
```

## 提示
### 制約

- $ p,\ q $ は `A`,`B`,`C`,`D`,`E`,`F`,`G` のいずれか
- $ p\ \neq\ q $
 
### Sample Explanation 1

点 $ A $ と点 $ C $ の距離は $ 3\ +\ 1\ =\ 4 $ です。

### Sample Explanation 2

点 $ G $ と点 $ B $ の距離は $ 9\ +\ 5\ +\ 1\ +\ 4\ +\ 1\ =\ 20 $ です。

