## ��Ŀ����
Farmer John is thinking of selling some of his land to earn a bit of extra income. His property contains $N$ trees ($3 \leq N \leq 300$), each described by a point in the 2D plane, no three of which are collinear. FJ is thinking about selling triangular lots of land defined by having trees at their vertices; there are of course $L = \binom{N}{3}$ such lots he can consider, based on all possible triples of trees on his property.

A triangular lot has value $v$ if it contains exactly $v$ trees in its interior (the trees on the corners do not count, and note that there are no trees on the boundaries since no three trees are collinear). For every $v = 0 \ldots N-3$, please help FJ determine how many of his $L$ potential lots have value $v$.

## �����ʽ
The first line of input contains $N$.

The following $N$ lines contain the $x$ and $y$ coordinates of a single tree; these are both integers in the range $0 \ldots 1,000,000$.

## �����ʽ
Output $N-2$ lines, where output line $i$ contains a count of the number of lots having value $i-1$.

## ��Ŀ����
### ��Ŀ����

Farmer John ���ڿ��ǳ�������һ����������׬ȡһЩ�������롣���ĲƲ����� $N$ ������$3 \leq N \leq 300$����ÿ�����ɶ�άƽ���е�һ���������������������������ߡ�FJ ���ڿ��ǳ�������������Ϊ���㶨��������εؿ飻��Ȼ�������Կ��ǵĴ���ؿ�����Ϊ $L = \binom{N}{3}$���������Ʋ������п��ܵ���������ϡ�

һ�������εؿ�ļ�ֵΪ $v$����������ڲ�ǡ�ð��� $v$ �����������ϵ��������룬������û�����������ߣ��߽���Ҳû������������ÿ�� $v = 0 \ldots N-3$������� FJ ȷ������ $L$ ��Ǳ�ڵؿ����ж��ٸ��ؿ�ļ�ֵΪ $v$��

### �����ʽ

����ĵ�һ�а��� $N$��

�������� $N$ ��ÿ�а���һ������ $x$ �� $y$ ���ꣻ��Щ���궼�� $0 \ldots 1,000,000$ ��Χ�ڵ�������

### �����ʽ

��� $N-2$ �У����е� $i$ �������ֵΪ $i-1$ �ĵؿ�������

```input1
7
3 6
17 15
13 15
6 12
9 1
2 7
10 19
```

```output1
28
6
1
0
0
```

