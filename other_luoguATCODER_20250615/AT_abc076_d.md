# AT_abc076_d [ABC076D] AtCoder Express

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc076/tasks/abc076_d

$ 2168 $年、AtCoder 社は成長し、ついに "AtCoder特急" という鉄道を建設することを決めた。

さて、社長の高橋君は、"AtCoder特急" の列車を以下のように運行することを計画した。

- 列車の走行時間は、$ (t_1\ +\ t_2\ +\ t_3\ +\ ...\ +\ t_N) $ 秒である。
- 最初の $ t_1 $ 秒間は、列車は速度 $ v_1 $ m/s 以内で走っていなければならない。また、次の $ t_2 $ 秒間は、列車は速度 $ v_2 $ m/s 以内で走っていなければならない。 次の $ t_3 $ 秒間、またそれ以降についても同様である。
- 最後の $ t_N $ 秒間は、列車は速度 $ v_N $ m/s 以内で走っていなければならない。

ただし、列車の性能上、加速度は ±$ 1m/s^2 $ 以内でなければならない。また、走行開始時と走行終了時には列車は止まっていなければならない。

列車が発車してから停車するまでに走れる最大の距離を求めなさい。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ t_1 $ $ t_2 $ $ t_3 $ … $ t_N $ $ v_1 $ $ v_2 $ $ v_3 $ … $ v_N $

## 输出格式

列車が発車してから停車するまでに走ることのできる最大の距離を出力しなさい。 ただし、絶対誤差が $ 10^{-3} $ 以内であれば、正解となります。

## 输入输出样例 #1

### 输入 #1

```
1
100
30
```

### 输出 #1

```
2100.000000000000000
```

## 输入输出样例 #2

### 输入 #2

```
2
60 50
34 38
```

### 输出 #2

```
2632.000000000000000
```

## 输入输出样例 #3

### 输入 #3

```
3
12 14 2
6 2 7
```

### 输出 #3

```
76.000000000000000
```

## 输入输出样例 #4

### 输入 #4

```
1
9
10
```

### 输出 #4

```
20.250000000000000000
```

## 输入输出样例 #5

### 输入 #5

```
10
64 55 27 35 76 119 7 18 49 100
29 19 31 39 27 48 41 87 55 70
```

### 输出 #5

```
20291.000000000000
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ t_i\ \leq\ 200 $
- $ 1\ \leq\ v_i\ \leq\ 100 $
- 入力はすべて整数である

### Sample Explanation 1

![](https://img.atcoder.jp/abc076/69c1f4241b608bc36f1f08dd4184d3f0.png) - 最初の $ 30 $ 秒は、加速度を $ 1m/s^2 $ にし、加速します。その間に列車は $ 450m $ 走ります。 - 次の $ 40 $ 秒は、速度 $ 30m/s $ を保ちます。その間に列車は $ 1200m $ 走ります。 - 最後の $ 30 $ 秒は、加速度を $ -1m/s^2 $ にし、減速します。その間に列車は $ 450m $ 走ります。 合計で、$ 450 $ + $ 1200 $ + $ 450 $ = $ 2100m $ 走ることができます。

### Sample Explanation 2

![](https://img.atcoder.jp/abc076/a3e07ea723f50df04461165bc2cc8890.png) - 最初の $ 34 $ 秒は、加速度を $ 1m/s^2 $ にし、加速します。その間に列車は $ 578m $ 走ります。 - 次の $ 26 $ 秒は、速度 $ 34m/s $ を保ちます。その間に列車は $ 884m $ 走ります。 - 次の $ 4 $ 秒は、加速度を $ 1m/s^2 $ にし、加速します。その間に列車は $ 144m $ 走ります。 - 次の $ 8 $ 秒は、速度 $ 38m/s $ を保ちます。その間は列車は $ 304m $ 走ります。 - 最後の $ 38 $ 秒は、加速度を $ -1m/s^2 $ にし、減速します。その間に列車は $ 722m $ 走ります。 合計で、$ 578 $ + $ 884 $ + $ 144 $ + $ 304 $ + $ 722 $ = $ 2632m $ 走ることができます。

### Sample Explanation 3

![](https://img.atcoder.jp/abc076/77f821f590cb19d8e449303a102422dc.png) - 最初の $ 6 $ 秒は、加速度を $ 1m/s^2 $ にし、加速します。その間に列車は $ 18m $ 走ります。 - 次の $ 2 $ 秒は、速度 $ 6m/s $ を保ちます。その間に列車は $ 12m $ 走ります。 - 次の $ 4 $ 秒は、加速度を $ -1m/s^2 $ にし、減速します。その間に列車は $ 16m $ 走ります。 - 次の $ 14 $ 秒は、速度 $ 2m/s $ を保ちます。その間は列車は $ 28m $ 走ります。 - 最後の $ 2 $ 秒は、加速度を $ -1m/s^2 $ にし、減速します。その間に列車は $ 2m $ 走ります。 合計で、$ 18 $ + $ 12 $ + $ 16 $ + $ 28 $ + $ 2 $ = $ 76m $ 走ることができます。

### Sample Explanation 4

![ ](https://img.atcoder.jp/abc076/ebde8cbeb649ae7fd338180c0562ae0b.png) - 最初の $ 4.5 $ 秒は、加速度を $ 1m/s^2 $ にし、加速します。その間に列車は $ 10.125m $ 走ります。 - 最後の $ 4.5 $ 秒は、加速度を $ -1m/s^2 $ にし、減速します。その間に列車は $ 10.125m $ 走ります。 合計で、$ 10.125 $ + $ 10.125 $ = $ 20.25m $ 走ることができます。