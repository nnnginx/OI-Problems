## 题目描述
Lily White is playing with strings. Being a yousei, she is not capable of complex speech. Thus, she likes strings that only contain one kind of letter, she calls such strings of length $x$ a "$x$-CON string". For example, `qqqq` is a "$4$-CON string", while `aaab` is not any type of "CON string".

Lily White composed an array $a$. It contains $n$ strings of length $m$ that she will use to herald spring. For each permutation of $1,2,\ldots, n$, let us denote current permutation as $p=\{p_1,p_2,\cdots,p_n\}$. Lily White concatenates all the string in array $a$ in the order of $a_{p_1},a_{p_2},\cdots,a_{p_n}$ into a string $s$ of length $nm$ . 

As she likes $k$-CON strings, she wants to know the sum of the number of "$k$-CON string" in all non-empty substrings of $s$ composed by all $n!$ permutations. Since the answer may be enormous, just print the answer taken modulo $998,244,353$ (a large prime).


## 输入格式
The first line contains three integers $n,m,k$.

Then $n$ lines follow, each line contains a string of length $m$. The string in the$(i+1)$-th line represents $a_i$.

## 输出格式
Print a single integer - the answer taken modulo $998,244,353$.


## 题目大意
给定若干长度为 $m$ 的字符串 $a_1,a_2,...,a_n$，给定常数 $k$，试求出对于所有的长度为 $n$ 的排列 $p$，将 $a_{p_1},a_{p_2},...,a_{p_n}$ 依次拼接形成的长字符串 $s$ 中，有多少个位置 $x$ 满足 $s_x,s_{x+1},...,s_{x+k-1}$ 为同一种字符。请输出位置数的和 $\bmod \space998244353$ 的值。

```input1
3 3 5
aaa
baa
baa

```

```output1
4
```

```input2
3 3 2
xyz
qaq
aba

```

```output2
0
```

```input3
5 3 2
cca
cbb
acb
bbb
acb

```

```output3
600
```

```input4
5 3 5
aba
bbb
bbb
aba
bcb

```

```output4
120
```

## 提示
### Explanation

#### Sample \#1

- For permutation $1,2,3$, the formed $s$ is `aaabaabaa`, none on the non-empty substring in this string are "$5$-CON string".
- For permutation $1,3,2$, the formed $s$ is `aaabaabaa`, none on the non-empty substring in this string are "$5$-CON string".
- For permutation $2,1,3$, the formed $s$ is `baaaaabaa`, this string has one substring `aaaaa` which is a "$5$-CON string".
- For permutation $2,3,1$, the formed $s$ is `baabaaaaa`, this string has one substring `aaaaa` which is a "$5$-CON string".
- For permutation $3,1,2$, the formed $s$ is `baaaaabaa`, this string has one substring `aaaaa` which is a "$5$-CON string".
- For permutation $3,2,1$, the formed $s$ is `baabaaaaa`, this string has one substring `aaaaa` which is a "$5$-CON string".

In summary, the answer is $0+0+1+1+1+1=4$.

#### Sample \#2

In all of the full permutation of length $3$, there will be six different $s$: `xyzqaqaba`, `xyzabaqaq`, `qaqxyzaba`, `qaqabaxyz`, `abaqaqxyz`, and `abaxyzqaq`. None of these has a non-empty substrings which is a "$2$-CON string". So the answer is $0$.

### Constraints

$2\le k \le n\cdot m\le 10^6;\ 1\le m \le 100$. $a_i$ contains only lowercase English letters.

