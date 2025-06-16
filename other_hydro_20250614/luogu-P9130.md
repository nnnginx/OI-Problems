## ��Ŀ����
**Note: The time limit for this problem is 6s, three times the default. The memory limit for this problem is 512MB, twice the default.** 

Bessie is a hungry cow. Each day, for dinner, if there is a haybale in the barn, she will eat one haybale. Farmer John does not want Bessie to starve, so some days he sends a delivery of haybales, which arrive in the morning (before dinner). In particular, on day $d_i$, Farmer John sends a delivery of $b_i$ haybales $(1 \le d_i \le 10^{14}, 0 \le b_i \le 10^9)$.

Process $U(1 \le U \le 10^5)$ updates as follows: Given a pair $(d,b)$, update the number of haybales arriving on day $d$ to $b$. After each update, output the sum of all days on which Bessie eats haybales modulo $10^9+7$. 

## �����ʽ
$U$, followed by $U$ lines containing the updates. 

## �����ʽ
The sum after each update modulo $10^9+7$. 

## ��Ŀ����
Bessie �ܶ���ÿ��������иɲݾͻ�� $1$ �ݣ�û�оͲ��ԣ���ʼû�иɲݡ�

ÿ������ Farmer John ����������ɸɲݣ���� $k$ ���� $a_k$ �ݸɲݣ���ʼʱ $a_k=0$����ʾ���첻�͸ɲݡ�

$q$ �β�����ÿ�θ��� $x,y$����ʾ�� $a_x$ �ĳ� $y$���뽫�ڴ�ʱ Bessie �иɲݳԵ�**���ڱ��**��Ͳ�������� $10^9+7$ ȡģ��

�����以��������

$1\le q\le10^5$��$1\le x\le10^{14}$��$0\le y\le10^9$��

```input1
3
4 3
1 5
1 2
```

```output1
15
36
18
```

```input2
9
1 89
30 7
101 26
1 24
5 1
60 4
5 10
101 0
1 200
```

```output2
4005
4656
7607
3482
3507
3753
4058
1107
24531
```

## ��ʾ
### Explanation for Sample 1

Answers after each update:

$4+5+6=15$  
$1+2+3+4+5+6+7+8=36$  
$1+2+4+5+6=18$

### SCORING

 - Input $3$: $U \le 5000$
 - Inputs $4-10$: Updates only increase the number of haybales arriving on day $d$.
 - Inputs 11-22: No additional constraints.

