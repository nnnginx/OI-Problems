## ��Ŀ����

Bessie has been playing with strings again. She found that by changing the order of the alphabet she could make some strings come before all the others lexicographically (dictionary ordering). For instance Bessie found that for the strings $\tt omm$, $\tt moo$, $\tt mom$, and $\tt ommnom$ she could make $\tt mom$ appear first using the standard alphabet and that she could make $\tt omm$ appear first using the alphabet $\tt abcdefghijklonmpqrstuvwxyz$. However, Bessie couldn't figure out any way to make $\tt moo$ or $\tt ommnom$ appear first.

Help Bessie by computing which strings in the input could be lexicographically first by rearranging the order of the alphabet. To compute if string $X$ is lexicographically before string $Y$ find the index of the first character in which they differ, $j$. If no such index exists then $X$ is lexicographically before $Y$ if $X$ is shorter than $Y$. Otherwise $X$ is lexicographically before $Y$ if $X[j]$ occurs earlier in the alphabet than $Y[j]$.

��Ŀ���⣺���� $n$ ���ܳ������� $m$ �Ļ�����ͬ���ַ������������������ָ���ַ�֮��Ĵ�С��ϵ�����ж��ٸ������ܳ�Ϊ�ֵ�����С�Ĵ����������Щ����

## �����ʽ

Line 1: A single line containing $n$, the number of strings Bessie is playing with.

Lines 2..1+n: Each line contains a non-empty string. The total number of characters in all strings will be no more than $3\times 10^5$. All characters in input will be lowercase characters $\tt a$ through $\tt z$. Input will contain no duplicate strings.

## �����ʽ

Line 1: A single line containing $k$, the number of strings that could be lexicographically first.

Lines 2..1+k: The 1+i th line should contain the $i$th string that could be lexicographically first. Strings should be output in the same order they were given in the input.

## ��������

```
4
omm
moo
mom
ommnom
```

## �������

```
2
omm
mom
```

## ��ʾ

INPUT DETAILS: The example from the problem statement.

OUTPUT DETAILS: Only $\tt omm$ and $\tt mom$ can be ordered first.

## ���ݹ�ģ��Լ��

����100%�����ݣ�$n \leq 3\times 10^4$�� $m \leq 3\times 10^5$��

