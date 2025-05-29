## ��Ŀ����
``gshfd1jkhaRaadfglkjerVcvuy0gf`` said Prof. Pang. 

To understand Prof. Pang's word, we would like to calculate the number of $\textit{namomo subsequence}$s of it. The word by Prof. Pang is a string $s$ with $n$ characters where each character is either an English letter (lower or upper case) or a digit. The $i$-th character of $s$ is denoted by $s[i]$ ($1\le i\le n$). A subsequence $t$ of $s$ is defined by a list of indices $t_1, \ldots, t_6$ such that $1\le t_1 < t_2 < \ldots < t_6\le n$. Let $compare(c_1, c_2)$ be a function on two characters such that $compare(c_1, c_2)=1$ when $c_1=c_2$ and $compare(c_1, c_2)=0$ otherwise. $t$ is a namomo subsequence of $s$ if and only if for any $1\le i<j\le 6$, $compare(s[t_i], s[t_j]) = compare(namomo[i], namomo[j])$, where $namomo[x]$ represents the $x$-th character of the string ``namomo`` ($1\le x\le 6$). 

Output the number of namomo subsequences of a given string $s$ modulo $998244353$.

## �����ʽ
The first line contains a string $s$ with $n$ characters ($6\le n\le 1000000$). $s$ contains only lower case English letters (`a` -- `z`), upper case English letters (`A` -- `Z`) and digits (`0` -- `9`).

## �����ʽ
Output one integer -- the answer modulo $998244353$.

## ��Ŀ����
����һ���� $s$�������ж��ٸ�����Ϊ $6$ ������ $A B C D C D$ �������С� 

$6\le |s|\le 10^6$���ַ�����С $62$��

```input1
wohaha
```

```output1
1
```

```input2
momomo
```

```output2
0
```

```input3
gshfd1jkhaRaadfglkjerVcvuy0gf
```

```output3
73
```

```input4
retiredMiFaFa0v0
```

```output4
33
```

