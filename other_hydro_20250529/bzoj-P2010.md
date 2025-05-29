## ��Ŀ����

Ϊ��֤�᳡��ȫ��ר��ȷ����ÿһ��ÿһ�еı������������Ϣ��һ��ѹ������ʽ������ȷ���Ƿ��п���ʵ������һ�ַ�������ÿ��ÿ�а���ȷ�������ı��ڡ�������λ������ǿյģ�Ҳ����˵�������Ա�����������һ����λ�ϡ� ��Ŀ�ȼ�����֪һ�� $01$ �����ÿ�С�ÿ�и��ж��ٸ� $1$���������ľ����Ƿ���ڡ�

�������ݹ���Ϊ���� $r$ ���������� $a_1,b_1,a_2,b_2, \ldots a_r,b_r$ ��ʾ��� $01$ ����һ���� $b_1+b_2+ \ldots +b_r$ �У������� $b_i$ ���ж����� $a_i$ �� $1$�� ͬ���ģ��� $c$ ���������� $p_i$ �� $q_i$ ����ʾ�е��� Ϣ��

## �����ʽ

The input begins with the description of the rows. The first line of the input contains one positive integer $r$ : the number of groups of rows. $r$ lines follow. Each of these lines contains $2$ positive integers: the required number of bodyguards in each row of the group and the number of rows that form the group. This is followed by the description of column groups. The next line contains one positive integer $c$ : the number of groups of columns. $c$ lines follow. Each of these lines contains $2$ positive integers: the required number of bodyguards in each column of the group and the number of columns that form the group.

## �����ʽ

Output a single line with the number `1` if the constraints are satisfiable and the number `0` otherwise.

```input1
2
2 1
1 2
1
2 2
```
```output1
1
```

## ����˵�� 1
There are two groups of rows: the first one has one row that must contain two bodyguards, the second one has two rows that must contain one bodyguard each. There is one group of columns: each of the two columns must contain two bodyguards. One possible placement of bodyguards:

```
 XX
 X.
 .X
```

```input2
2
3 2
1 1
2
3 2
1 1
```
```output2
0
```

## ����˵�� 2

Two of the rows are required to be full of bodyguards. Hence there must be at least two bodyguards in each column. However, the last column must only contain one bodyguard, which is a contradiction.

## ���ݹ�ģ��Լ��

���� $50\%$ �����ݣ�$r,c\le 2\times10^3$������� $10^6$ �����ڡ�

���� $100\%$ �����ݣ������������Ϊ $10^{18}$���������־�Ϊ���������Ҳ����� $10^9$��$1\le r,c\le 2\times 10^5$�����ݱ�֤���кͰ��м�����ܱ�������ȡ�