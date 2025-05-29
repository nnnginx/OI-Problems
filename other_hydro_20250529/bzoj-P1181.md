## ��Ŀ����

��һ��������ѡ���У����� $v$ ���˲μ���ͶƱ��ÿһƱֻ����Ͷ�� $n$ �������е�һ�������ص���Ṳ�� $m$ ��ϯλ�������� $n$ ���������Ϊ $1$ �� $n$����������Ϊ $i$ ���������յĵ�ƱΪ $v_i$��������е�ϯλ�����¹�����䣺

1. ����Ʊ��С����ѡƱ�� $5\%$ �������޳���
2. ��ʼʱ���Ϊ�գ�ÿ��������ֻ�� $0$ ��ϯλ��
3. ����ÿ������ $p$������һ������ $q_p = v_p / (s_p + 1)$��$v_p$ Ϊ���� $p$ �����յ�Ʊ��$s_p$ Ϊ���� $p$ ��ǰ�Ѿ������ӵ�е�ϯλ��
4. �� $q_p$ ������������һ��ϯλ������ж�������� $q_p$ ��ͬ����ϯλ�ָ����б����С��������
5. �ظ� $3$ �� $4$��ֱ�����������

���ڼ�Ʊ��û�н�������������ֻ֪��һ����ѡƱ��ͶƱ��������� $v��n��m$ �Լ�ÿ��������ǰ�ĵ�Ʊ���������ÿ����������Լ�������Ӯ�ö��ٸ�ϯλ��


```input1
20 4 5
4 3 6 1
```

```output1
3 3 3 2
1 0 1 0
```


## ��ʾ

14 votes have been tallied and 6 are yet to be counted. 

To illustrate one possible outcome, suppose that the first party receives 2 of those 6 votes, the second none, the third 1 vote and the fourth 3 votes. The parties' totals are 6, 3, 7 and 4 votes. 

All parties exceeded the 5% threshold. Seats are allocated as follows: 

1. The quotients are initially 6/1, 3/1, 7/1 and 4/1; the largest is 7/1 so party 3 wins a seat. 
2. The quotients are 6/1, 3/1, 7/2 and 4/1; the largest is 6/1 so party 1 wins a seat. 
3. The quotients are 6/2, 3/1, 7/2 and 4/1; the largest is 4/1 so party 4 wins a seat. 
4. The quotients are 6/2, 3/1, 7/2 and 4/2; the largest is 7/2 so party 3 wins a seat. 
5. The quotients are 6/2, 3/1, 7/3 and 4/2; parties 1 and 2 are tied with quotients 6/2 and 3/1, but party 1 is lower numbered so it wins the last seat. 

In this outcome, the numbers of seats won by the parties are 2, 0, 2 and 1. Since it is possible for the second party not to win any seats, the second number on the second line of output is zero.

## ���ݹ�ģ��Լ��


���� $100\%$ �����ݣ�$1 \le v \le 1\times 10^7�� 1 \le n \le 100�� 1 \le m \le 200$��
