# AT_abc089_b [ABC089B] Hina Arare

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc089/tasks/abc089_b

日本では、$ 3 $ 月 $ 3 $ 日にひなあられという、色のついたお菓子をお供えする習慣があります。

$ 1 $ つの袋があり、ひなあられが $ N $ 個入っています。

この袋には、桃色、白色、緑色の $ 3 $ 種類か、桃色、白色、緑色、黄色の $ 4 $ 種類のひなあられが入っていることが分かっています。

桃色を `P`、白色を `W`、緑色を `G`、黄色を `Y` と表したとき、袋からひなあられを $ 1 $ 粒ずつ取り出していったところ、$ i $ 番目に取り出したひなあられの色は $ S_i $ でした。

この袋に $ 3 $ 種類のひなあられが入っていた場合は `Three`、$ 4 $ 種類のひなあられが入っていた場合は `Four` と出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ ... $ $ S_N $

## 输出格式

袋に $ 3 $ 種類のひなあられが入っていた場合は `Three`、$ 4 $ 種類のひなあられが入っていた場合は `Four` と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
6
G W Y P Y W
```

### 输出 #1

```
Four
```

## 输入输出样例 #2

### 输入 #2

```
9
G W W G P W P G G
```

### 输出 #2

```
Three
```

## 输入输出样例 #3

### 输入 #3

```
8
P Y W G Y W Y Y
```

### 输出 #3

```
Four
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ S_i $ は `P` か `W` か `G` か `Y`
- $ S_i= $`P`、$ S_j= $`W`、$ S_k= $`G` を満たす $ i,j,k $ が必ず存在する

### Sample Explanation 1

袋に $ 4 $ 種類のひなあられが入っていたので `Four` と出力するとよいです。

### Sample Explanation 2

袋に $ 3 $ 種類のひなあられが入っていたので `Three` と出力するとよいです。