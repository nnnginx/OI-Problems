## ��Ŀ����
**���� [JOI Open 2016](https://contests.ioi-jp.org/open-2016/index.html) T2 ��RNA �i��؜�� / Selling RNA Strands��**

�������ڲ������ݹ��࣬���ڴ��ṩ���ֲ������ݣ�ʣ��������[�ڴ˲���](https://www.luogu.com.cn/problem/U288877)��

## ��Ŀ����
��������� $N$ ���ַ�������Щ�ַ������� `A`��`G`��`U`��`C` ��ɣ���֤ÿ���ַ���������������ĸ����

�� $M$ ���ѯ��ÿ���ѯ���������ַ��� $P,Q$�����󣺻�������ж��ٸ��ַ���ͬʱ����ǰ׺ $P$ �ͺ�׺ $Q$��

�ٸ����ӣ�`GAC` ����ǰ׺ `G`��`GA`��`GAC`�����ں�׺ `C`��`AC`��`GAC`����ô���ǿ���˵��`GAC` ͬʱ����ǰ׺ `GA` �ͺ�׺ `AC`��

## �����ʽ
���빲 $N + M + 1$ �С�

��һ������������ $N, M$��  
�ڽ������� $N$ ���У�ÿ��һ���ַ��� $S_i$����ʾ������е�һ���ַ�����  
�ڽ������� $M$ ���У�ÿ���������ÿո�ָ����ַ�������ʾһ���ѯ��

## �����ʽ
����� $M$ �У�ÿ��һ����������ʾ���ϲ�ѯ�������ַ�����������

```input1
2 3
AUGC
AGC
G C
AU C
A C
```

```output1
0
1
2
```

```input2
3 3
AA
AA
AGA
AA AA
AG GA
AG GA
```

```output2
2
1
1
```

```input3
8 7
GCGCUACCCCAACACAAGGCAAGAUAUA
G
GGAC
GCGG
U
GCGCUACCCCAACACAAGGCAAGAUGGUC
GCCG
GCGCUGA
GCGCUACCC A
GCGCUACCCC AC
GCG C
GCGC A
G G
G C
G GGA
```

```output3
1
0
1
2
3
2
0
```

## ��ʾ
### ���� 1 ����

��һ���ѯ���޷��ҵ���  
�ڶ����ѯ��`AUGC` ����������  
�������ѯ��`AUGC` �� `AGC` ����������

### ���� 2 ����

ע�������е��ַ��������ظ���

### ���ݹ�ģ��Լ��

**��������������**��

�����������ݣ�$1\le N, M \leq 10 ^ 5$��$1 \leq |S_i|, |P_j|, |Q_j| \le 10^5$��$1\le\sum |S_i|, \sum |P_j|, \sum |Q_j| \le 2\times 10^6$��

- Subtask 1��10 points����$N, M, |S_i|, |P_j|, |Q_j| \le 100$��
- Subtask 2��25 points����$N, M\le 5000$��
- Subtask 3��25 points����$\sum |S_i|, \sum|P_j|, \sum |Q_j| \le 10^5$��
- Subtask 4��40 points����û�ж������ơ�

