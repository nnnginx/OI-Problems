# AT_joi2015ho_e 城壁 (Rampart)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/joi2015ho/tasks/joi2015ho_e

歴史学者である JOI 教授は，かつて存在した IOI 王国について研究している．

過去の調査によると，IOI 王国は縦 $ H $ 行，横 $ W $ 列のマスに区切られた長方形の形をしていた．IOI 王国の首都は，防衛のために城壁で囲われていた．

IOI 王国の首都を囲う城壁は次のような形をしている．城壁には大きさと呼ばれる値が定まっている．大きさ $ s $ ($ s\ \geqq\ 3 $) の城壁とは，$ s\ \times\ s $ の正方形の領域から外周以外の $ (s\ -\ 2)\ \times\ (s\ -\ 2) $ の正方形の領域を除いたものである．

調査によると，首都を囲う城壁の大きさは $ L $ 以上であった．また，IOI 王国のいくつかのマスには城壁が存在しなかったことがわかっている．

JOI 教授は，さらなる研究のために，城壁としてありうるものが何通りあるかを知りたい．

## 输入格式

標準入力から以下のデータを読み込め．

- $ 1 $ 行目には，整数 $ H,\ W,\ L,\ P $ が空白を区切りとして書かれている．これは，IOI 王国は縦 $ H $ 行，横 $ W $ 列のマスに区切られた長方形の形をしており，城壁の大きさは $ L $ 以上であり，城壁が存在しなかったことがわかっているマスが $ P $ マス存在することを表す．
- 続く $ P $ 行のうちの $ i $ 行目 ($ 1\ \leqq\ i\ \leqq\ P $) には，整数 $ A_i,\ B_i $ が空白を区切りとして書かれている．これは，IOI 王国の上から $ A_i $ 行目，左から $ B_i $ 列目のマスには城壁が存在しなかったことがわかっていることを表す．

## 输出格式

標準出力に，城壁としてありうるものは何通りあるかを表す整数を $ 1 $ 行で出力せよ．

- - - - - -

## 输入输出样例 #1

### 输入 #1

```
5 5 3 2
2 2
4 3
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
7 8 4 3
2 2
3 7
6 5
```

### 输出 #2

```
13
```

## 输入输出样例 #3

### 输入 #3

```
4000 4000 1234 4
1161 3028
596 1892
3731 2606
702 1530
```

### 输出 #3

```
7050792912
```

## 说明/提示

### 課題

IOI 王国の大きさと，城壁の大きさの最小値，城壁が存在しなかったことが分かっているマスの情報が与えられたとき，城壁としてありうるものは何通りあるかを求めるプログラムを作成せよ．

- - - - - -

### 制限

すべての入力データは以下の条件を満たす．

- $ 1\ \leqq\ H\ \leqq\ 4\,000 $．
- $ 1\ \leqq\ W\ \leqq\ 4\,000 $．
- $ 3\ \leqq\ L\ \leqq\ H $ かつ $ 3\ \leqq\ L\ \leqq\ W $．
- $ 0\ \leqq\ P\ \leqq\ 100\,000 $．
- $ 1\ \leqq\ A_i\ \leqq\ H $ ($ 1\ \leqq\ i\ \leqq\ P $)．
- $ 1\ \leqq\ B_i\ \leqq\ W $ ($ 1\ \leqq\ i\ \leqq\ P $)．
- ($ A_i,\ B_i)\ \neq\ (A_j,\ B_j $) ($ 1\ \leqq\ i\ <\ j\ \leqq\ P $)．

### 小課題

#### 小課題 1 \[4 点\]

以下の条件を満たす．

- $ H\ \leqq\ 500 $．
- $ W\ \leqq\ 500 $．

#### 小課題 2 \[16 点\]

- $ 0\ \leqq\ P\ \leqq\ 10 $ を満たす．

#### 小課題 3 \[80 点\]

追加の制限はない．

- - - - - -

### Sample Explanation 1

この入力例の場合，城壁としてありうるものは以下の $ 4 $ 通りが考えられる．ただし，`×` で示したマスは城壁が存在しなかったことがわかっているマスである． !\[e-1.png\](https://img.atcoder.jp/joi2015ho/e-1.png) - - - - - -

### Sample Explanation 2

\- - - - - -