## ��Ŀ����
Given $n$ strings $w_1, w_2, \cdots, w_n$, please select $k$ strings among them, so that the lexicographic order of string $v$ is minimized, and output the optimal string $v$. String $v$ satisfies the following constraint: $v$ is the longest common prefix of two selected strings with different indices. Also, $v$ is the lexicographically largest string among all strings satisfying the constraint.

More formally, let $\mathbb{S}$ be a set of size $k$, where all the elements in the set are integers between $1$ and $n$ (both inclusive) and there are no duplicated elements. Let $\text{lcp}(w_i, w_j)$ be the longest common prefix of string $w_i$ and $w_j$, please find a set $\mathbb{S}$ to minimize the lexicographic order of the following string $v$ and output the optimal string $v$.

$$
v = \max\limits_{i \in \mathbb{S}, j \in \mathbb{S}, i \ne j} \text{lcp}(w_i, w_j)
$$

In the above expression, $\max$ is calculated by comparing the lexicographic order of strings.

Recall that:
- String $p$ is a prefix of string $s$, if we can append some number of characters (including zero characters) at the end of $p$ so that it changes to $s$. Specifically, empty string is a prefix of any string.
- The longest common prefix of string $s$ and string $t$ is the longest string $p$ such that $p$ is a prefix of both $s$ and $t$. For example, the longest common prefix of ``abcde`` and ``abcef`` is ``abc``, while the longest common prefix of ``abcde`` and ``bcdef`` is an empty string.
- String $s$ is lexicographically smaller than string $t$ ($s \ne t$), if
  - $s$ is a prefix of $t$, or
  - $s_{|p| + 1} < t_{|p| + 1}$, where $p$ is the longest common prefix of $s$ and $t$, $|p|$ is the length of $p$, $s_i$ is the $i$-th character of string $s$, and $t_i$ is the $i$-th character of string $t$.
- Specifically, empty string is the string with the smallest lexicographic order.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $k$ ($2\leq n\leq 10^6$, $2\leq k\leq n$) indicating the total number of strings and the number of strings to be selected.

For the following $n$ lines, the $i$-th line contains a string $w_i$ ($1\leq |w_i|\leq 10^6$) consisting of lower-cased English letters.

It's guaranteed that the total length of all strings of all test cases will not exceed $10^6$.

## �����ʽ
For each test case output one line containing one string indicating the answer. Specifically, if the answer is an empty string, print $\texttt{EMPTY}$.

## ��Ŀ����
**����Ŀ������**

���� $n$ ���ַ��� $w_1, w_2, \cdots, w_n$����ѡ��ǡ�� $k$ ���ַ�������С���ַ��� $v$ ���ֵ��򣬲����������ŵ��ַ��� $v$������ $v$ ��������������$v$ �Ǳ�ѡ�����ַ����У�ĳ������Ų�ͬ���ַ����������ǰ׺�����ң�$v$ �����������������ַ����У��ֵ��������ַ�����

����ʽ�أ��� $\mathbb{S}$ ��ʾһ����СΪ $k$ �ļ��ϣ������е�Ԫ�ؾ�Ϊ�� $1$ �� $n$ �������������ˣ�����û���ظ���Ԫ�ء��� $\text{lcp}(w_i, w_j)$ ��ʾ�ַ��� $w_i$ �� $w_j$ �������ǰ׺������Ҫ�ҵ�һ������ $\mathbb{S}$ ����С�������ַ��� $v$ ���ֵ��򣬲����������ŵ��ַ��� $v$��

$$
v = \max\limits_{i \in \mathbb{S}, j \in \mathbb{S}, i \ne j} \text{lcp}(w_i, w_j)
$$

��ʽ�е� $\max$ ͨ���ֵ���Ƚ������ַ�����

����䣺
- ���ַ��� $p$ ���ַ��� $s$ ��ǰ׺���������� $p$ ��ĩβ������ɸ��ַ�����������ַ���������� $s$���ر�أ����ַ����������ַ�����ǰ׺��
- �ַ��� $s$ �� $t$ �������ǰ׺��һ������ַ��� $p$������ $p$ ���� $s$ ��ǰ׺������ $t$ ��ǰ׺�����磬``abcde`` ��``abcef`` �������ǰ׺Ϊ ``abc``���� ``abcde`` �� ``bcdef`` �������ǰ׺Ϊ���ַ�����
- ���ַ��� $s$ ���ֵ���С���ַ��� $t$��$s \ne t$������
  - $s$ �� $t$ ��ǰ׺����
  - $s_{|p| + 1} < t_{|p| + 1}$������ $p$ Ϊ $s$ �� $t$ �������ǰ׺��$|p|$ Ϊ $p$ �ĳ��ȣ�$s_i$ ��ʾ�ַ��� $s$ �ĵ� $i$ ���ַ���$t_i$ ��ʾ�ַ��� $t$ �ĵ� $i$ ���ַ���
- �ر�أ����ַ������ֵ�����С���ַ�����

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$ ��ʾ������������������ÿ��������ݣ�

��һ�������������� $n$ �� $k$��$2\leq n\leq 10^6$��$2\leq k\leq n$������ʾ�ַ�������������Ҫѡ����ַ�����������

���ڽ����� $n$ �У��� $i$ ������һ����Сд��ĸ���ɵ��ַ��� $w_i$��$1\leq |w_i|\leq 10^6$����

��֤�����������ַ�������֮�Ͳ����� $10^6$��

**�������ʽ��**

ÿ���������һ��һ���ַ�����ʾ�𰸡��ر�أ�����Ϊ���ַ�������� $\texttt{EMPTY}$��

```input1
2
5 3
gdcpc
gdcpcpcp
suasua
suas
sususua
3 3
a
b
c
```

```output1
gdcpc
EMPTY
```

