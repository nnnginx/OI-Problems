## ����

��������������̺��Ȼ��һλ�������Ӳ�ͬ�⣬�͸�����ǰ׺�ˡ�

## ����

�������� $n$ ��һ������Ϊ $n$ ���ַ��� $s$ ������������ $a_i$ Ϊ $s$ ��ǰ $i$ ���ַ��� `A` �ĸ������������� $b_i$ Ϊ $s$ ��ǰ $i$ ���ַ��� `B` �ĸ�����

��֤ $\forall s_i\in \{A,B\}$ ��

���峤��Ϊ $n$ ������ $r_i$ ������

$$
r_i=\begin{cases}
0 & a_i=b_i\\
1 & a_i>b_i\\
-1 & a_i<b_i
\end{cases}
$$

���� $n-1$ �β��������е� $i$ �β������� $s_i$ �� $s_{i+1}$ ��**�����к�Ч��**�������� $a_i,b_i,r_i$ ���ܻᷢ���仯��

��¼��ʼ�� $r$ ���к�ÿ�β������ $r$ ���У������ռ�¼���˶����ֲ�ͬ�� $r$ ���С�

��������������ͬ�����鲻ͬ�����ҽ���������������������һ�Դ��ڶ�Ӧλ���ϵ�������ȡ�

## �����ʽ

��һ��һ������ $n$ ��

�ڶ���һ������Ϊ $n$ ���ַ��� $s$ ��

## �����ʽ

��һ��һ����������ʾ�𰸡�

## ����

```input1
4
AABB
```

```output1
3
```

```input2
4
AAAA
```

```output2
1
```

```input3
10
BBBAAABBAA
```

```output3
5
```

```input4
172
AABAAAAAABBABAABBBBAABBAAABBABBABABABBAAABAAABAABAABBBBABBBABBABBBBBBBBAAABAAABAAABABBBAABAAAABABBABBABBBBBABAABAABBBABABBAAAABAABABBBABAAAABBBBABBBABBBABAABBBAAAABAAABAAAB
```

```output4
24
```

## ���ݷ�Χ

���� $20\%$ �����ݣ���֤ $1\le n\le 3\times 10^3$ ��

�����������ݣ���֤ $1\le n\le 10^6$ ��

