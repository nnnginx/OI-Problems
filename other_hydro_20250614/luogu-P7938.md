## ��Ŀ����
In this problem, we define a sequence of `(` and `)` as a "bracket sequence".

The definition of *Regular Bracket Sequence* is as follows:

1. `()` is a Regular Bracket Sequence.
1. If `A` is a Regular Bracket Sequence, then `(A)` is also a Regular Bracket Sequence.
1. If `A` and `B` are Regular Bracket Sequences, then `AB` is also a Regular Bracket Sequence.

For example: `()`, `(())`, and `()()` are all Regular Bracket Sequences, but `)(`, `()(` are not.

In particular, an empty sequence is **not** a Regular Bracket Sequence sequence in this problem.

Now ~~cute~~ Ran gives you a bracket sequence $s$ of length $n$. She wants you to construct $2\cdot m$ **strictly increasing** arrays. Let us denote them as
 $p_1,p_2,\cdots,p_{2 m}$ (you can leave any of them empty). You need to ensure that all integers between $1\sim n$ appear **exactly once** in these arrays. 
 
An array $p_i=\{r_1,r_2,\cdots,r_k\}$ is *Beautiful* if    $\{s_{r_1},s_{r_2},\cdots,s_{r_k}\}$ is a Regular Bracket Sequence.

Ran wonders whether it is possible to construct these arrays so that at least $m$ of the $2\cdot m$ arrays are "beautiful arrays". 

## �����ʽ
Each test contains multiple test cases.

The first line contains an integer $T$, the number of test cases.

For each test case, the first line contains two integers $n$ and $m$, and the second line contains a bracket sequence $s$.

## �����ʽ
For each test case, print one line.

If it is possible to construct these arrays, print $1$. Otherwise print $0$.

## ��Ŀ����
����һ���ַ���Ϊ���Ŵ����ҽ�������� `(` �� `)` ��ɡ�

�Խ�һ������Ϊ $n$ �����Ŵ���Ϊ $2m$ �������У������п���Ϊ�գ���ÿ���ַ�������ֵ�ǡ��һ���������У�ʹ������ $m$ ��������Ϊƥ������Ŵ���**�����в���ƥ�����������**���޽������ $0$��������� $1$������������ݣ�������������Ϊ $T$��

���� $A$ Ϊ $B$ �������е��ҽ��� $A$ ���� $B$ ��˳�򲻸ı��ǰ����ɾ������Ԫ�غ�õ���

*���� $1$ ���ͣ�����Խ���һ���͵ڶ����ַ������һ�������У��õڶ���������Ϊ�������С���ʱ��һ��������Ϊ `()`���ڶ���Ϊ�գ��ܼ���һ��ƥ����������У�����Ҫ��

```input1
2
2 1
()
2 99
()
```

```output1
1
0
```

## ��ʾ
### Explanation

For the first test case, we can construct $p_1=\{1,2\}$ and $ p_2=\{\}$. So $p_1$ is a "beautiful array".

For the second test case, it is obvious that we cannot use two numbers to construct $99$ beautiful arrays.

### Constraints

$1\le T,n,m\le 200$.

