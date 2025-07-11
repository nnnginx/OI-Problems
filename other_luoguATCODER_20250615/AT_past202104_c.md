# AT_past202104_c 携帯電話の購入

## 题目描述

[problemUrl]: https://atcoder.jp/contests/past202104-open/tasks/past202104_c

ある会社は $ N $ 種類の携帯電話を販売しています。これらの機種は機種 $ 1 $ から機種 $ N $ まで番号づけられています。  
 また、携帯電話の周波数帯が $ M $ 個あり、周波数帯 $ 1 $ から周波数帯 $ M $ まで番号づけられています。  
 機種 $ i $ の携帯電話は周波数帯 $ A_{i,\ 1},\ A_{i,\ 2},\ A_{i,\ 3},\ \dots,\ A_{i,\ K_i} $ の $ K_i $ 個の周波数帯のみに対応しています。  
 あなたはこの会社の携帯電話のうち以下の条件を満たすものから $ 1 $ つ選んで買うことに決めました。

- 周波数帯 $ B_1,\ B_2,\ B_3,\ \dots,\ B_P $ の $ P $ 個の周波数帯のうち $ Q $ 個以上に対応している

あなたの買う携帯電話の候補となる機種の数を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K_1 $ $ A_{1,\ 1} $ $ A_{1,\ 2} $ $ A_{1,\ 3} $ $ \dots $ $ A_{1,\ K_1} $ $ K_2 $ $ A_{2,\ 1} $ $ A_{2,\ 2} $ $ A_{2,\ 3} $ $ \dots $ $ A_{2,\ K_2} $ $ K_3 $ $ A_{3,\ 1} $ $ A_{3,\ 2} $ $ A_{3,\ 3} $ $ \dots $ $ A_{3,\ K_3} $ $ \hspace{67pt}\ \vdots $ $ K_N $ $ A_{N,\ 1} $ $ A_{N,\ 2} $ $ A_{N,\ 3} $ $ \dots $ $ A_{N,\ K_N} $ $ P $ $ Q $ $ B_1 $ $ B_2 $ $ B_3 $ $ \dots $ $ B_P $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 4
1 4
2 3 1
3 2 1 3
2 2 4
2 1
2 4
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
4 4
3 2 3 4
1 2
2 1 3
4 1 2 3 4
3 1
1 3 4
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
1 2
1 1
1 1
2
```

### 输出 #3

```
0
```

## 说明/提示

### 注意

この問題に対する言及は、2021/4/24 18:00 JST まで禁止されています。言及がなされた場合、賠償が請求される可能性があります。 試験後に総合得点や認定級を公表するのは構いませんが、どの問題が解けたかなどの情報は発信しないようにお願いします。

### 制約

- $ 1\ \le\ N\ \le\ 50 $
- $ 1\ \le\ M\ \le\ 50 $
- $ 1\ \le\ K_i\ \le\ M $
- $ 1\ \le\ A_{i,\ j}\ \le\ M $
- $ j\ \neq\ k $ ならば $ A_{i,\ j}\ \neq\ A_{i,\ k} $
- $ 1\ \le\ Q\ \le\ P\ \le\ M $
- $ 1\ \le\ B_i\ \le\ M $
- $ i\ \neq\ j $ ならば $ B_i\ \neq\ B_j $
- 入力は全て整数

### Sample Explanation 1

それぞれの機種が対応している周波数は以下の通りです。 - 機種 $ 1 $ : 周波数帯 $ 4 $ - 機種 $ 2 $ : 周波数帯 $ 1,\ 3 $ - 機種 $ 3 $ : 周波数帯 $ 1,\ 2,\ 3 $ - 機種 $ 4 $ : 周波数帯 $ 2,\ 4 $ 周波数帯 $ 2,\ 4 $ のうち $ 1 $ 個以上に対応している機種は、機種 $ 1,\ 3,\ 4 $ です。

### Sample Explanation 2

機種 $ 1,\ 3,\ 4 $ が条件を満たします。

### Sample Explanation 3

$ 1 $ つも条件を満たす機種がない場合もあります。