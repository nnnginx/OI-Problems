# AT_abc113_d [ABC113D] Number of Amidakuji

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc113/tasks/abc113_d

あみだくじは, 日本に古くから伝わる伝統的なくじ引きである.

あみだくじを作るには, まず $ W $ 本の平行な縦線を引き, 次にそれらを繋ぐ横線を引いていく. それぞれの縦棒の長さは $ H+1 $ \[cm\] であり、横線の端点となれるのは上から $ 1,2,3,...,H $ \[cm\] の位置のみである.

ここで,「正しいあみだくじ」とは, 以下のような条件を満たすあみだくじのことである.

- どの $ 2 $ つの横棒も端点を共有しない.
- それぞれの横棒の $ 2 $ つの端点は同じ高さになければならない.
- 横棒は隣り合う縦線を繋がなければならない.

![ ](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc113_d/76ad4dbaf6281d141632ee1be437fcd6eb62cf06.png)

縦棒 $ 1 $ の上端から, 横線があれば必ずそれを通るというルールで下へたどったときに, 最終的にたどり着く縦棒の番号が $ K $ となるような「正しいあみだくじ」の本数を $ 1\ 000\ 000\ 007 $ で割った余りを求めなさい.

例として, 以下のあみだくじにおいて, 最終的にたどり着く縦棒の番号は $ 4 $ である.

![ ](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc113_d/798f2b4676c5cd94b2fff66ef18034da71e67ad6.png)

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ K $

## 输出格式

条件を満たすあみだくじの本数を $ 1\ 000\ 000\ 007 $ で割った余りを出力しなさい.

## 输入输出样例 #1

### 输入 #1

```
1 3 2
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
1 3 1
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
2 3 3
```

### 输出 #3

```
1
```

## 输入输出样例 #4

### 输入 #4

```
2 3 1
```

### 输出 #4

```
5
```

## 输入输出样例 #5

### 输入 #5

```
7 1 1
```

### 输出 #5

```
1
```

## 输入输出样例 #6

### 输入 #6

```
15 8 5
```

### 输出 #6

```
437760187
```

## 说明/提示

### 制約

- $ H $ は $ 1 $ 以上 $ 100 $ 以下の整数
- $ W $ は $ 1 $ 以上 $ 8 $ 以下の整数
- $ K $ は $ 1 $ 以上 $ W $ 以下の整数

### Sample Explanation 1

以下の $ 1 $ 個のあみだくじのみが条件を満たす. !\[ \](https://img.atcoder.jp/abc113/c68c6daccfc4cba8bc94af5f1a80ef2f.png)

### Sample Explanation 2

以下の $ 2 $ 個のあみだくじのみが条件を満たす. !\[ \](https://img.atcoder.jp/abc113/4be150946de8bef9b14d9bc17814d963.png)

### Sample Explanation 3

以下の $ 1 $ 個のあみだくじのみが条件を満たす. !\[ \](https://img.atcoder.jp/abc113/9b2e9f49832458c3488b1e04afd51ed4.png)

### Sample Explanation 4

以下の $ 5 $ 個のあみだくじのみが条件を満たす. !\[ \](https://img.atcoder.jp/abc113/bf6ec766f8923ac2f082f538a6c736b6.png)

### Sample Explanation 5

縦線が $ 1 $ 本しかないので, 横線をそもそも引くことができない. よって条件を満たすあみだくじは「一本も横線を引かない」の $ 1 $ 通りしかない.

### Sample Explanation 6

答えを $ 1\ 000\ 000\ 007 $ で割った余りを出力すること.