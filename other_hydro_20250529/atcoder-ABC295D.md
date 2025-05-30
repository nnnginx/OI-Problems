## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc295/tasks/abc295_d

`20230322` は並べ替えると `02320232` となり、これは `0232` を $ 2 $ 度繰り返しています。  
 このように、数字のみからなる文字列であって、適切に文字を並び替える (そのままでもよい) ことによって同じ列を $ 2 $ 度繰り返すようにできるものを **嬉しい列** と呼びます。  
 数字のみからなる文字列 $ S $ が与えられるので、以下の条件を全て満たす整数の組 $ (l,r) $ はいくつあるか求めてください。

- $ 1\ \le\ l\ \le\ r\ \le\ |S| $ ( $ |S| $ は $ S $ の長さ)
- $ S $ の $ l $ 文字目から $ r $ 文字目までの (連続する) 部分文字列は嬉しい列である。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを整数として出力せよ。

## 题目大意
给出一个数字串，问有多少子段满足，可以以某种方式将这个子段重排，将子段分成两个完全相同的部分。

```input1
20230322
```

```output1
4
```

```input2
0112223333444445555556666666777777778888888889999999999
```

```output2
185
```

```input3
3141592653589793238462643383279502884197169399375105820974944
```

```output3
9
```

## 提示
### 制約

- $ S $ は数字のみからなる長さ $ 1 $ 以上 $ 5\ \times\ 10^5 $ 以下の文字列
 
### Sample Explanation 1

$ S= $ `20230322` です。 条件を満たす整数組 $ (l,r) $ は $ (1,6),(1,8),(2,7),(7,8) $ の $ 4 $ つです。

### Sample Explanation 2

$ S $ の先頭が `0` である場合もあります。

