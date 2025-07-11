# AT_abc374_c [ABC374C] Separated Lunch

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc374/tasks/abc374_c

キーエンス本社に勤務する人数が増えてきたので、本社に存在する部署を $ 2 $ つのグループに分け、昼休みの時間帯を分けることにしました。

キーエンス本社には $ N $ 個の部署が存在し、$ i $ 番目 $ (1\leq\ i\leq\ N) $ の部署に所属する人数は $ K_i $ 人です。

それぞれの部署をグループ $ A $, $ B $ のいずれか一方に割り当て、グループごとに同時に昼休みをとり、 かつグループ $ A $, $ B $ の昼休みの時間が重ならないようにしたとき、同時に昼休みをとる最大人数としてあり得る最小の値を求めてください。  
 すなわち、グループ $ A $ に割り当てられた部署に所属する人数の合計とグループ $ B $ に割り当てられた部署に所属する人数の合計 のうち大きい方の値としてあり得る最小の値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K_1 $ $ K_2 $ $ \ldots $ $ K_N $

## 输出格式

同時に昼休みを取る最大人数としてあり得る最小の値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
2 3 5 10 12
```

### 输出 #1

```
17
```

## 输入输出样例 #2

### 输入 #2

```
2
1 1
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
6
22 25 26 45 22 31
```

### 输出 #3

```
89
```

## 说明/提示

### 制約

- $ 2\leq\ N\ \leq\ 20 $
- $ 1\leq\ K_i\ \leq\ 10^8 $
- 入力はすべて整数
 
### Sample Explanation 1

$ 1,2,5 $ 番目の部署をグループ $ A $ に、$ 3,4 $ 番目の部署をグループ $ B $ に割り当てたとき、 グループ $ A $ に割り当てられた部署に所属する人数の合計は $ 2+3+12=17 $ 、 グループ $ B $ に割り当てられた部署に所属する人数の合計は $ 5+10=15 $ となり、 このとき同時に昼休みを取る最大人数は $ 17 $ となります。 一方で、グループ $ A,B $ それぞれに割り当てられた部署に所属する人数の合計がいずれも $ 16 $ 以下になるように 部署を割り当てることはできないため、$ 17 $ を出力します。

### Sample Explanation 2

同一人数の部署が複数存在する可能性もあります。

### Sample Explanation 3

例えば、$ 1,4,5 $ 番目の部署をグループ $ A $ に、$ 2,3,6 $ 番目の部署をグループ $ B $ に割り当てたとき同時に昼休みを取る最大人数は $ 89 $ となります。