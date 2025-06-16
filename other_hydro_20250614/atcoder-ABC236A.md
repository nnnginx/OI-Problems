## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc236/tasks/abc236_a

英小文字からなる文字列 $ S $ が与えられます。

$ S $ の先頭から $ a $ 文字目と $ b $ 文字目を入れ替えて得られる文字列を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $ $ a $ $ b $

## 输出格式
答えを出力せよ。

## 题目大意
# 输入格式
输入一个字符串 $S(2\le|S|\le10)$和两个正整数 $a,b(1\le a,b\le|s|)$。

# 输出格式
将这个字符串的第 $a$ 和第 $b$ 个字符调换后输出。

**记得换行！！**

```input1
chokudai
3 5
```

```output1
chukodai
```

```input2
aa
1 2
```

```output2
aa
```

```input3
aaaabbbb
1 8
```

```output3
baaabbba
```

## 提示
### 制約

- $ S $ は英小文字からなる文字列
- $ S $ の長さ $ |S| $ は、 $ 2\ \leq\ |S|\ \leq\ 10 $ を満たす
- $ 1\ \leq\ a\ <\ b\ \leq\ |S| $
- $ a,\ b $ は整数

### Sample Explanation 1

`chokudai` の $ 3 $ 文字目 `o` と $ 5 $ 文字目 `u` を入れ替えると `chukodai` となります。

### Sample Explanation 2

この入力例では、$ S $ の $ 1 $ 文字目と $ 2 $ 文字目を入れ替えて得られる文字列は、元の $ S $ と同じになります。

