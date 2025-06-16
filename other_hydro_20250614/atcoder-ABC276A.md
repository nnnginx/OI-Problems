## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc276/tasks/abc276_a

英小文字からなる文字列 $ S $ が与えられます。  
 $ S $ に `a` が現れるならば最後に現れるのが何文字目かを出力し、現れないならば $ -1 $ を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを出力せよ。

## 题目大意
输入一个由小写英文字母构成的字符串 $S$，如果字符串中有 `a` 就输出位置最靠右的 `a` 的下标（下标从 $1$ 开始），否则就输出 $-1$。  

$1\le\vert S \vert\le 100$。

```input1
abcdaxayz
```

```output1
7
```

```input2
bcbbbz
```

```output2
-1
```

```input3
aaaaa
```

```output3
5
```

## 提示
### 制約

- $ S $ は英小文字からなる長さ $ 1 $ 以上 $ 100 $ 以下の文字列

### Sample Explanation 1

$ S $ に `a` は $ 3 $ 回現れますが、最後に現れるのは $ 7 $ 文字目なので、$ 7 $ を出力します。

### Sample Explanation 2

$ S $ に `a` は現れないので、$ -1 $ を出力します。

