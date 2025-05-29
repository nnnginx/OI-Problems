## ��Ŀ����
Farmer John owns 3\*N (1 <= N <= 500,000) cows surprisingly numbered 0..3\*N-1, each of which has some associated integer weight W\_i (1 <= W\_i <= d). He is entering the Grand Farm-off, a farming competition where he shows off his cows to the greater agricultural community.

This competition allows him to enter a group of N cows. He has given each of his cows a utility rating U\_i (1 <= U\_i <= h), which

represents the usefulness he thinks that a particular cow will have in the competition, and he wants his selection of cows to have the maximal sum of utility.

There might be multiple sets of N cows that attain the maximum utility sum. FJ is afraid the competition may impose a total weight limit on the cows in the competition, so a secondary priority is to bring lighter weight competition cows.

Help FJ find a set of N cows with minimum possible total weight among the sets of N cows that maximize the utility, and print the remainder when this total weight is divided by M (10,000,000 <= M <= 1,000,000,000).

Note: to make the input phase faster, FJ has derived polynomials which will generate the weights and utility values for each cow. For each cow 0 <= i < 3\*N,

 $$W_i=(a\times i^5+b\times i^2+c)\mod d$$
 
 $$U_i=(e\times i^5+f\times i^3+g)\mod h$$
 
 $$(0\le a,b,c,d,e,f,g,h\le 10^9)$$

The formulae do sometimes generate duplicate numbers; your algorithm should handle this properly. 

ũ��Լ����3N(1 < N < 500000)ͷţ���������Ϊ1..#N��ÿͷţ����һ������ֵ���� �ء�Լ��׼���μ�ũ�����մ����������ũҵ����չʾ������ţ.
������������Լ����Nͷţ����.Լ����ÿͷţ������һ�������öȡ�Ui������ ʾ��ĳͷţ�ڱ����е����ó̶�.Լ��ϣ����ѡ������ţ�����ö�֮�����.

�п���ѡ���ܶ����Nͷţ���ܴﵽ���ö�����.Լ������ѡ����Nͷţ��������������� �����𺳣����ԣ�Ҫ��������ѡ�����������ţ.

����Լ��ѡ��Nͷ���������ᣬ�������ö�֮��������ţ.�������ģM�������.

ע�⣺Ϊ��ʹ������죬Լ��ʹ����һ������ʽ������ÿͷţ�����غ����ö�.��ÿͷţ/�� ���غ����öȵļ��㹫ʽΪ��



 $$W_i=(a\times i^5+b\times i^2+c)\mod d$$
 
 $$U_i=(e\times i^5+f\times i^3+g)\mod h$$
 
 $$(0\le a,b,c,d,e,f,g,h\le 10^9)$$

## �����ʽ
\* Line 1: Ten space-separated integers: N, a, b, c, d, e, f, g, h, and M


## �����ʽ
\* Line 1: A single integer representing the lowest sum of the weights of the N cows with the highest net utility.


```input1
2 0 1 5 55555555 0 1 0 55555555 55555555 

```

```output1
51 

```

## ��ʾ
The functions generate weights of 5, 6, 9, 14, 21, and 30 along with utilities of 0, 1, 8, 27, 64, and 125.


The two cows with the highest utility are cow 5 and 6, and their combined weight is 21+30=51.


