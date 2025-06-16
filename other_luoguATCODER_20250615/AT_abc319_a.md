# AT_abc319_a [ABC319A] Legendary Players

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc319/tasks/abc319_a

AtCoder では、レーティング上位 $ 10 $ 人のハンドルネームには金色の冠が、上位 $ 1 $ 人のハンドルネームには白金色の冠が表示されます。

このコンテストが開始した時点で、アルゴリズム部門での上位 $ 10 $ 人に入っているプレイヤーのハンドルネームとレーティングは以下のようになっています。

```
<pre class="prettyprint" id="username_rating" style="padding: 9.5px; border: 1px solid #ccc;">
tourist 3858
ksun48 3679
Benq 3658
Um_nik 3648
apiad 3638
Stonefeang 3630
ecnerwala 3613
mnbvmar 3555
newbiedmy 3516
semiexp 3481
```

上記のプレイヤーのハンドルネーム $ S $ が与えられるので、その人のレーティングを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

対応するプレイヤーのレーティングを $ 1 $ 行で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
tourist
```

### 输出 #1

```
3858
```

## 输入输出样例 #2

### 输入 #2

```
semiexp
```

### 输出 #2

```
3481
```

## 说明/提示

### 制約

- $ S $ はアルゴリズム部門でレーティング上位 $ 10 $ 人に入っているプレイヤーのハンドルネームのいずれかと等しい。

### Sample Explanation 1

このコンテストが開始した時点において、!\[\](//img.atcoder.jp/assets/icon/crown\_champion.png) \[tourist\](/users/tourist) さんのアルゴリズム部門のレーティングは $ 3858 $ です。

### Sample Explanation 2

このコンテストが開始した時点において、!\[\](//img.atcoder.jp/assets/icon/crown\_gold.png) \[semiexp\](/users/semiexp) さんのアルゴリズム部門のレーティングは $ 3481 $ です。