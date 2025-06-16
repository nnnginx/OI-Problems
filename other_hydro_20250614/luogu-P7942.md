## ��Ŀ����
**In easy version, It is guaranteed that any string in array $\mathbf a$ contains at least two different letters.**

Lily White is playing with strings. Being a yousei, she is not capable of complex speech. Thus, she likes strings that only contain one kind of letter, she calls such strings of length $x$ a "$x$-CON string". For example, `qqqq` is a "$4$-CON string", while `aaab` is not any type of "CON string".

Lily White composed an array $a$. It contains $n$ strings of length $m$ that she will use to herald spring. For each permutation of $1,2,\ldots, n$, let us denote current permutation as $p=\{p_1,p_2,\cdots,p_n\}$. Lily White concatenates all the string in array $a$ in the order of $a_{p_1},a_{p_2},\cdots,a_{p_n}$ into a string $s$ of length $nm$ . 

As she likes $k$-CON strings, she wants to know the sum of the number of "$k$-CON string" in all non-empty substrings of $s$ composed by all $n!$ permutations. Since the answer may be enormous, just print the answer taken modulo $998,244,353$ (a large prime).


## �����ʽ
The first line contains three integers $n,m,k$.

Then $n$ lines follow, each line contains a string of length $m$. The string in the$(i+1)$-th line represents $a_i$.

## �����ʽ
Print a single integer - the answer taken modulo $998,244,353$.


## ��Ŀ����
**�� easy version �У���֤���� $\mathbf a$ �е��ַ������ٰ������ֲ�ͬ����ĸ��**

�������ɳ���Ϊ $m$ ���ַ��� $a_1,a_2,...,a_n$���������� $k$��������������еĳ���Ϊ $n$ ������ $p$���� $a_{p_1},a_{p_2},...,a_{p_n}$ ����ƴ���γɵĳ��ַ��� $s$ �У��ж��ٸ�λ�� $x$ ���� $s_x,s_{x+1},...,s_{x+k-1}$ Ϊͬһ���ַ��������λ�����ĺ� $\bmod \space998244353$ ��ֵ��

```input1
3 3 4
aab
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

## ��ʾ
### Explanation

#### Sample \#1

- For permutation $1,2,3$, the formed $s$ is `aabbaabaa`, none on the non-empty substring in this string are "$4$-CON string".
- For permutation $1,3,2$, the formed $s$ is `aabbaabaa`, none on the non-empty substring in this string are "$4$-CON string".
- For permutation $2,1,3$, the formed $s$ is `baaaabbaa`, this string has one substring `aaaa` which is a "$4$-CON string".
- For permutation $2,3,1$, the formed $s$ is `baabaaaab`, this string has one substring `aaaa` which is a "$4$-CON string".
- For permutation $3,1,2$, the formed $s$ is `baaaabbaa`, this string has one substring `aaaa` which is a "$4$-CON string".
- For permutation $3,2,1$, the formed $s$ is `baabaaaab`, this string has one substring `aaaa` which is a "$4$-CON string".

In summary, the answer is $0+0+1+1+1+1=4$.

#### Sample \#2

In all of the full permutation of length $3$, there will be six different $s$: `xyzqaqaba`, `xyzabaqaq`, `qaqxyzaba`, `qaqabaxyz`, `abaqaqxyz`, and `abaxyzqaq`. None of these has a non-empty substrings which is a "$2$-CON string". So the answer is $0$.

### Constraints

$2\le k \le n\cdot m\le 10^6;\ 1\le m \le 100$. $a_i$ contains only lowercase English letters.

**In easy version, we ensure that any string in array $\mathbf a$ contains at least two different letters.**

