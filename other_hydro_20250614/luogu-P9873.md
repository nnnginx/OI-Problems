## ��Ŀ����
Prof. Pang recently got a dictionary of the elvish language, including many strings representing their words. He thinks a partition of string $s$ is beautiful if both of the following conditions are satisfied:

- $s = s_1 + s_2 + s_3 + s_4 + s_5 + s_6$, where $s_i (1\leq i\leq 6)$ are nonempty substrings. $a + b$ means the concatenation of string $a$ and $b$ here.
- $s_1 = s_2 = s_5, s_3 = s_6$.


For example, you can partition the string ``114514`` into $6$ parts : ``114514`` = ``1`` + ``1`` + ``4`` + ``5`` + ``1`` + ``4``. The first, second, fifth parts are the same, and the third and sixth parts are the same. Thus, the partition of $s=$``114514`` into $s_1=$``1``, $s_2=$``1``, $s_3=$``4``, $s_4=$``5``, $s_5=$``1``, and $s_6=$``4`` is beautiful. 

Accordingly, the beauty of a string $s$ is defined as the number of beautiful partitions of $s$.

Given a string $t$, please help Prof. Pang to figure out the sum of beauties of all substrings of $t$.


## �����ʽ
The first line contains a single integer $T~(1\leq T \le 50)$ indicating the number of test cases. 

For each test case, there is one single line containing the string $t$, consisting of digits from `0' to `9'.

It is guaranteed that the length of each $t$ in each test case will not exceed $5000$ and the total length will not exceed $30000$.

## �����ʽ
For each test case, output a single line containing an integer, indicating the sum of beauties of all substrings of $t$.

## ��Ŀ����
���ַ��� $s$ ��һ��**����**��������������

- $s = s_1 + s_2 + s_3 + s_4 + s_5 + s_6$������ $s_i (1\leq i\leq 6)$ Ϊ�ǿ��Ӵ���$a + b$ ��ʾ���ַ��� $b$ ���� $a$ ��

- $s_1 = s_2 = s_5, s_3 = s_6$��

��Ƹ�**����**��**������**��

�ַ��� $s$ ��**����ֵ**����Ϊ $s$ �Ĳ�ͬ��**�����Ļ���**�ĸ�����

�����ַ��� $s$������**�����Ӵ�**��**����ֵ֮��**��

```input1
2
114514
0000000
```

```output1
1
3
```

