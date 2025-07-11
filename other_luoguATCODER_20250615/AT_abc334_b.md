# AT_abc334_b [ABC334B] Christmas Trees

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc334/tasks/abc334_b

東西に無限に伸びる道路があり、この道路上のある基準となる地点から東に $ x\mathrm{\,m} $ のところにある地点の**座標**は $ x $ と定められています。 特に、基準となる地点から西に $ x\mathrm{\,m} $ のところにある地点の座標は $ -x $ です。

すぬけ君は今から、座標が $ A $ である地点を基点にして $ M\mathrm{\,m} $ おきにクリスマスツリーを立てます。 すなわち、座標がある整数 $ k $ を用いて $ A+kM $ と表されるような地点それぞれにクリスマスツリーを立てます。

高橋君と青木君はそれぞれ座標が $ L,R\ (L\leq\ R) $ である地点に立っています。 高橋君と青木君の間（高橋君と青木君が立っている地点を含む）に立てられるクリスマスツリーの本数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ M $ $ L $ $ R $

## 输出格式

高橋君と青木君の間（高橋君と青木君が立っている地点を含む）に立てられるクリスマスツリーの本数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 3 -1 6
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
-2 2 1 1
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
-177018739841739480 2436426 -80154573737296504 585335723211047198
```

### 输出 #3

```
273142010859
```

## 说明/提示

### 制約

- $ -10^{18}\leq\ A\ \leq\ 10^{18} $
- $ 1\leq\ M\ \leq\ 10^9 $
- $ -10^{18}\leq\ L\leq\ R\ \leq\ 10^{18} $
- 入力は全て整数

### Sample Explanation 1

すぬけ君は、座標が $ \dots,-4,-1,2,5,8,11,14\dots $ である地点にクリスマスツリーを立てます。 これらのうち高橋君と青木君の間にあるのは、座標が $ -1,2,5 $ である地点に立てられる $ 3 $ 本です。

### Sample Explanation 2

高橋君と青木君が同じ地点に立っていることもあります。