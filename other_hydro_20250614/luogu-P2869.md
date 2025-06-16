## ��Ŀ����
Like so many others, the cows have developed very haughty tastes and will no longer graze on just any grass. Instead, Farmer John must purchase gourmet organic grass at the Green Grass Grocers store for each of his N (1 �� N �� 100,000) cows.

Each cow i demands grass of price at least Ai (1 �� Ai �� 1,000,000,000) and with a greenness score at least Bi (1 �� Bi �� 1,000,000,000). The GGG store has M (1 �� M �� 100,000) different types of grass available, each with a price Ci (1 �� Ci �� 1,000,000,000) and a greenness score of Di (1 �� Di �� 1,000,000,000). Of course, no cow would sacrifice her individuality, so no two cows can have the same kind of grass.

Help Farmer John satisfy the cows' expensive gourmet tastes while spending as little money as is necessary.

## �����ʽ
\* Line 1: Two space-separated integers: N and M.

\* Lines 2..N+1: Line i+1 contains two space-separated integers: Ai and Bi

\* Lines N+2..N+M+1: Line i+N+1 contains two space-separated integers: Ci and Di


## �����ʽ
\* Line 1: A single integer which is the minimum cost to satisfy all the cows. If that is not possible, output -1.


## ��Ŀ����
### ��Ŀ����

Լ������ţ��ʳ��Խ��Խ�����ˡ����ڣ��̵��� $m$ �����ݿɹ����ۣ���ţʳ���ܴ�ÿ�����ݽ��ܹ�һͷ��ţʳ�á��� $i$ �����ݵļ۸�Ϊ $p_i$���ڸ�Ϊ $q_i$��

Լ��һ���� $n$ ͷ��ţ����ҪΪÿͷ��ţ����һ�����ݣ��� $i$ ͷ��ţҪ�� �������ݼ۸񲻵��� $a_i$���ڸв����� $b_i$�����ʣ�Լ��Ӧ�����Ϊÿͷ��ţѡ�����ݣ�������������Ǯ���٣�

### �����ʽ

��һ�У��������� $n$ �� $m$��  

�� $2\sim n+1$ �У��� $i+1$ ���������� $a_i$ �� $b_i$��  

�� $n+2\sim n+m+1$ �У��� $i+n+1$ ���������� $c_i$ �� $d_i$��

���������������

### �����ʽ

�����һ�У������ܹ�����������ţҪ����Ҫ����Ǯ����Сֵ��������ܹ�����������ţ��Ҫ����� `-1`��

### ���ݷ�Χ

���� $100\%$ �����ݣ����� $1\leqslant n\leqslant 10^5$��$1\leqslant a_i,b_i,c_i,d_i\leqslant 10^9$��

```input1
4 7
1 1
2 3
1 4
4 2
3 2
2 1
4 3
5 2
5 4
2 6
4 4
```

```output1
12
```

