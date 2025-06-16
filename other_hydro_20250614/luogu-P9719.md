## ��Ŀ����
For a string $s$ of length $n$, we define $p_j = x$ if $s[x\ldots j]$ is the minimum suffix of $s[1\ldots j]$, for all $j=1,\ldots, n$. (A suffix is the minimum suffix of a string if it is lexicographically smaller than any other suffix of that string.)

You are to recover $s$ from $p_1,\ldots, p_n$. If there are multiple answers, find the lexicographically smallest one.

## �����ʽ
The first line contains a single integer $T$ ($1\le T\le 10^5$) representing the number of test cases.

For each test case, the first line contains a single integer $n$ ($1\le n\le 3\times 10^6$) representing the length of $s$. The next line contains $n$ integers $p_1,\ldots, p_n$ ($1\le p_i\le i$ for all $1\le i\le n$).

It is guaranteed that the sum of $n$ over all test cases does not exceed $3\times 10^6$.

## �����ʽ
For each test case, output one line. If there is no solution, output $-1$. Otherwise, output the lexicographically smallest $s$. Characters of $s$ are represented by positive integers. Smaller integers represent smaller characters in the lexicographical order.

## ��Ŀ����
**����Ŀ������**

���ڳ���Ϊ $n$ ���ַ��� $s$����� $s[x\ldots j]$ �� $s[1\ldots j]$ ����С��׺�������Ƕ��� $p_j = x$������ $j=1,\ldots, n$������׺���ַ�������С��׺����������ֵ�����С�ڸ��ַ������κ�������׺����

����Ҫ�� $p_1,\ldots, p_n$ �лָ��� $s$��������ڶ���𰸣����ҳ��ֵ�����С���Ǹ���

**�������ʽ��**

��һ�а���һ������ $T$��$1\le T\le 10^5$������ʾ����������������

����ÿ��������������һ�а���һ������ $n$��$1\le n\le 3\times 10^6$������ʾ $s$ �ĳ��ȡ���������һ�а��� $n$ ������ $p_1,\ldots, p_n$��$1\le p_i\le i$��$1\le i\le n$����

��֤���в��������� $n$ ���ܺͲ����� $3\times 10^6$��

**�������ʽ��**

����ÿ���������������һ�С����û�н������������� $-1$����������ֵ�����С�� $s$��$s$ �е��ַ�����������ʾ����С��������ʾ�ֵ����С���ַ���

**����ʾ˵����**

�������������ģ�ϴ󣬽���ʹ�ÿ��ٵ����������ʽ��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
6
3
1 1 1
3
1 1 2
3
1 1 3
3
1 2 1
3
1 2 2
3
1 2 3
```

```output1
1 2 2
-1
1 2 1
1 1 2
2 1 2
1 1 1
```

## ��ʾ
As the input/output can be huge, it is recommended to use fast input/output methods.

