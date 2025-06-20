# AT_tenka1_2016_qualA_c 山田山本問題

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tenka1-2016-quala/tasks/tenka1_2016_qualA_c

天下一株式会社に勤務するワタナベくんは、社内のコミュニケーションにチャットツールを使っています。 チャットツールには補完機能があり、@で始まるアカウント名を入力しようとすると、プレフィックスの一致するアカウント名の一覧を辞書順で補完候補として表示してくれます。

ところが、ワタナベくんは補完候補の中から @yamamoto を選ぼうとした時に、間違って @yamada を選択してしまうことが多々あります。 @yamada は @yamamoto より辞書順で小さく、 `@yama` まで入力した際に、候補の先頭に表示されてしまうためです。

ワタナベくんは不思議な特技を持っていて、アルファベットの順番を自由に並べ替えることができます。 例えば、ワタナベくんが特技を使ってアルファベットの順番を abcefghijklmdnopqrstuvwxyz にすると、 `m` は `d` より小さくなり、 @yamamoto を @yamada より辞書順で小さくすることができます。

アカウント名 $ A_i $ をアカウント名 $ B_i $ より辞書順で小さくしたいという要求が $ N $ 個与えられます。 与えられた要求をすべて満たすような、ワタナベくんの特技によって並べ替えられたアルファベットの順番を求めてください。 条件を満たすようなアルファベットの順番が複数存在する場合は、並べ替えられる前のアルファベットの順番での辞書順最小の順番を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ : $ A_N $ $ B_N $

## 输出格式

条件を満たすようなアルファベットの順番のうち、辞書順最小のものを1行に出力せよ。  
そのようなアルファベットの順番が存在しない場合は、-1を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1
yamamoto yamada
```

### 输出 #1

```
abcefghijklmdnopqrstuvwxyz
```

## 输入输出样例 #2

### 输入 #2

```
3
xx xy
z w
v w
```

### 输出 #2

```
abcdefghijklmnopqrstuvxyzw
```

## 输入输出样例 #3

### 输入 #3

```
2
a b
b a
```

### 输出 #3

```
-1
```

## 输入输出样例 #4

### 输入 #4

```
1
yamamoto yama
```

### 输出 #4

```
-1
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ A_i\ \neq\ B_i $
- $ 1\ \leq\ |A_i|,\ |B_i|\ \leq\ 1000 $
- $ A_i,B_i $は英小文字で構成される