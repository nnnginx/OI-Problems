## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc211/tasks/abc211_c

文字列 $ S $ が与えられます。  
 このうち $ 8 $ 文字を選び下線を引き、下線を引いた文字が左から順に `c` , `h` , `o` , `k` , `u` , `d` , `a` , `i` となるようにする方法は何通りありますか？  
 ただし答えは非常に大きくなる可能性があるので、$ (10^9\ +\ 7) $ で割った余りを出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを $ (10^9\ +\ 7) $ で割った余りを出力せよ。

## 题目大意
给定一个字符串，求有多少个非连续子串`chokudai`。

**注意：此处非连续子串的定义是：有字符串 $a,b$，如果从 $a$ 的任意位置删除若干个字符后可以得到 $b$，则称 $b$ 是 $a$ 的非连续子串。**

答案对 $10^9+7$ 取模。

```input1
chchokudai
```

```output1
3
```

```input2
atcoderrr
```

```output2
0
```

```input3
chokudaichokudaichokudai
```

```output3
45
```

## 提示
### 制約

- $ 8\ \leq\ |S|\ \leq\ 10^5 $
- $ S $ は英小文字からなる

### Sample Explanation 1

chchokudai chchokudai chchokudai 上の $ 3 $ つが条件を満たします。 chchokudai は、条件を満たさないことに注意してください。

### Sample Explanation 2

答えが $ 0 $ 通りになることもあります。

