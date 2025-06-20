# AT_relay2018_b ロボット

## 题目描述

[problemUrl]: https://atcoder.jp/contests/cf18-relay-open/tasks/relay2018_b

$ xy $ 平面上の点 $ (0,0) $ にロボットが $ 1 $ 個置かれています。 あなたは、このロボットに、`L`, `R`, `U`, `D` からなる文字列を $ 1 $ つ命令として与えることができます。 ロボットは文字列を与えられると、先頭の文字から順に、 `L` なら $ x $ 軸方向に $ -1 $、`R` なら $ x $ 軸方向に $ +1 $、`U` なら $ y $ 軸方向に $ +1 $、`D` なら $ y $ 軸方向に $ -1 $ 動くという動作を最後の文字まで行います。

あなたは、`W`,`X`,`Y`,`Z` からなる文字列 $ S $ を持っています。あなたは、これら $ 4 $ 種類の文字をそれぞれ `L` ,`R` ,`U` ,`D`のいずれかに置き換えた文字列を、ロボットに与えようとしています。 ただし、$ S $ において異なる文字を命令において同じ文字に割り当てることはできません。

文字列 $ S $ と整数 $ g_x,\ g_y $ が与えられます。 適切な文字の割り当てによってロボットが動き始めてから移動を終えるまで (開始、終了点を含みます) のどこかで座標 $ (g_x,g_y) $ を通るようにできるなら `Yes` を、できないなら `No` を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ g_x $ $ g_y $

## 输出格式

適切な文字の割り当てによってロボットが動き始めてから移動を終えるまで (開始、終了点を含みます) のどこかで座標 $ (g_x,g_y) $ を通るようにできるなら `Yes` を、できないなら `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
WWYWYWWW
3 0
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
YYYYW
-1 -3
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
WWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWW
0 50
```

### 输出 #3

```
Yes
```

## 说明/提示

### 制約

- $ 1\ <\ =\ |S|\ <\ =\ 10^5 $
- $ S $ は `W`, `X`, `Y`, `Z` からなる文字列
- $ |g_x|,\ |g_y|\ <\ =\ 10^5 $
- $ g_x,\ g_y $ は整数

### Sample Explanation 1

例えば、`W` を `R` に、`X` を `U` に、`Y` を `L` に、`Z` を `D` に割り当てることによって、$ (3,0) $ を通ることができます。