## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc224/tasks/abc224_a

末尾が `er` または `ist` であるような文字列 $ S $ が与えられます。  
 $ S $ の末尾が `er` である場合は `er` を、 `ist` である場合は `ist` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを出力せよ。

## 题目大意
输入一个字符串 $s$ ，在 $s$ 的末尾为 er 时输出 er ，在 $s$ 的末尾为 ist 时输出 ist 。保证 $s$ 的末尾为 er 或 ist 中的其中一种。

```input1
atcoder
```

```output1
er
```

```input2
tourist
```

```output2
ist
```

```input3
er
```

```output3
er
```

## 提示
### 制約

- $ 2\ \le\ |S|\ \le\ 20 $
- $ S $ は英小文字のみからなる。
- $ S $ の末尾は `er` または `ist` である。

### Sample Explanation 1

$ S= $"`atcoder`" の末尾は `er` です。

