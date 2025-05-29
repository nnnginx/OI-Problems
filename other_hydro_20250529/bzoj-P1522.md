## ��Ŀ����

���� $n$ ���� ${a_1,a_2,\cdots,a_n}$����һ������ ${b_1,b_2,\cdots,b_n}$ ���㣺

1.���� $b_i\le a_i$
2.$b_1\ xor\ b_2\ xor\ b_3\ xor\cdots xor\ bn=0$
3.$sum_{i=1}^{n}b_i>0$

���������еĸ�����

## �����ʽ

The first line of the standard input contains the number of elements $n$, $1\le n\le 50$.

The second, last line of the standard input contains $n$ positive integers $m_1,\cdots,m_n$, separated by single spaces,$1\le m_i < 2^{32}-1$.

## �����ʽ

Your programme should write one integer to the standard output - total number of different crystals that can be created. You can assume that this number is less than $2^{64}$.

```input1
3
2 1 3
```
```output1
5
```