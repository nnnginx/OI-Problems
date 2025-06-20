# AT_arc044_a [ARC044A] 素数判定

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc044/tasks/arc044_a

高橋君は素数判定アルゴリズムが大好きです。毎日さまざまな素数判定アルゴリズムを実装して遊んでいます。 しかし、高橋君は素数判定をしすぎてしまったので、素数判定に飽きてしまいました。 そこで高橋君は、「素数っぽく見える数」判定をすることにしました。

$ 1 $以上の整数$ N $は、以下のように「素数っぽい」かどうかが判定されます。

- $ N $が素数であるなら、$ N $は「素数っぽい」
- $ N $が合成数であるなら、$ N $を$ 10 $進表記した時の$ 1 $の位が偶数でも$ 5 $でもなく、各桁の和が$ 3 $で割り切れないならば、$ N $は「素数っぽい」
- それ以外の場合、$ N $は「素数っぽくない」

整数$ N $が与えられるので、$ N $が「素数っぽい」場合は"Prime"、そうでない場合は"Not Prime"と出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

- $ 1 $ 行目には、整数$ N(1\ ≦\ N\ ≦\ 10^9) $が与えられる。

## 输出格式

$ N $が「素数っぽい」場合は"Prime"、そうでない場合は"Not Prime"と出力せよ。

 出力の末尾に改行を入れること。(21:40修正)

## 输入输出样例 #1

### 输入 #1

```
42
```

### 输出 #1

```
Not Prime
```

## 输入输出样例 #2

### 输入 #2

```
49
```

### 输出 #2

```
Prime
```

## 输入输出样例 #3

### 输入 #3

```
3
```

### 输出 #3

```
Prime
```

## 输入输出样例 #4

### 输入 #4

```
1
```

### 输出 #4

```
Not Prime
```

## 说明/提示

### Sample Explanation 1

$ 42 $は合成数かつ$ 1 $の位が偶数なので、「素数っぽくない」と判定されます。

### Sample Explanation 2

$ 49 $は素数ではありませんが、「素数っぽい」と判定されます。

### Sample Explanation 3

$ 3 $は素数なので、「素数っぽい」と判定されます。

### Sample Explanation 4

$ 1 $は素数でも合成数でもないので、「素数っぽくない」と判定されます。