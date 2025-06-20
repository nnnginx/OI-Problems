# AT_keyence2020_a Painting

## 题目描述

[problemUrl]: https://atcoder.jp/contests/keyence2020/tasks/keyence2020_a

$ H $ 行 $ W $ 列の マス目があり、最初すべてのマスは白色です。

あなたは、このマス目に何回かペイント操作を施すことにしました。 $ 1 $ 回のペイント操作では、以下の $ 2 $ 種類の作業のうちいずれか $ 1 $ つが行えます。

- 行をひとつ選び、その行に含まれるマスをすべて黒く塗る。
- 列をひとつ選び、その列に含まれるマスをすべて黒く塗る。

黒く塗られているマスの個数が $ N $ 個以上となるようにするためには、最小で何回のペイント操作が必要ですか。 なお、制約の項で記述される条件のもとで、何回かペイント操作を行うことで 黒く塗られているマスの個数が $ N $ 個以上となるようにできることが保証されます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ N $

## 输出格式

ペイント操作の回数の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
7
10
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
14
12
112
```

### 输出 #2

```
8
```

## 输入输出样例 #3

### 输入 #3

```
2
100
200
```

### 输出 #3

```
2
```

## 说明/提示

### 制約

- $ 1\ \leq\ H\ \leq\ 100 $
- $ 1\ \leq\ W\ \leq\ 100 $
- $ 1\ \leq\ N\ \leq\ H\ \times\ W $
- 入力値はすべて整数である。

### Sample Explanation 1

「行をひとつ選び、その行に含まれるマスをすべて黒く塗る」という操作を異なる行に対して $ 1 $ 回ずつ、 合計 $ 2 $ 回行うことで、黒く塗られているマスの個数を $ 14 $ にできます。