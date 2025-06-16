# AT_abc056_a [ABC056A] HonestOrDishonest

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc056/tasks/abc056_a

シカのAtCoDeerくんとTopCoDeerくんが「正直者か嘘つきか」ゲームをしています。 このゲームでは、正直者は常にほんとうのことを言い、嘘つきは常に嘘を言います。 文字 $ a $ と $ b $ が入力として与えられます。これらはそれぞれ `H` か `D` のどちらかです。

$ a $=`H` のとき、AtCoDeerくんは正直者です。 $ a $=`D` のとき、AtCoDeerくんは嘘つきです。 $ b $=`H` のとき、AtCoDeerくんは「TopCoDeerくんは正直者だ」と発言しています。 $ b $=`D` のとき、AtCoDeerくんは「TopCoDeerくんは嘘つきだ」と発言しています。

これらから判断して、TopCoDeerくんが正直者かどうか判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $

## 输出格式

TopCoDeerくんが正直者なら `H` を、嘘つきなら `D` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
H H
```

### 输出 #1

```
H
```

## 输入输出样例 #2

### 输入 #2

```
D H
```

### 输出 #2

```
D
```

## 输入输出样例 #3

### 输入 #3

```
D D
```

### 输出 #3

```
H
```

## 说明/提示

### 制約

- $ a $=`H` または `D`
- $ b $=`H` または `D`

### Sample Explanation 1

AtCoDeerくんは正直者なので、AtCoDeerくんの言っているとおりTopCoDeerくんは正直者です。

### Sample Explanation 2

今度はAtCoDeerくんは嘘つきなので、AtCoDeerくんの言っていることとは異なりTopCoDeerくんは嘘つきです。