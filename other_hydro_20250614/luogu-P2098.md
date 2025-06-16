## ��Ŀ����
Every year, Farmer John brings his $N$ cows to compete for "best in show" at the state fair. His arch-rival, Farmer Paul, brings his $M$ cows to compete as well ($1 \leq N \leq 1000, 1 \leq M \leq 1000$).

Each of the $N + M$ cows at the event receive an individual integer score. However, the final competition this year will be determined based on teams of $K$ cows ($1 \leq K \leq 10$), as follows: Farmer John and Farmer Paul both select teams of $K$ of their respective cows to compete. The cows on these two teams are then paired off: the highest-scoring cow on FJ's team is paired with the highest-scoring cow on FP's team, the second-highest-scoring cow on FJ's team is paired with the second-highest-scoring cow on FP's team, and so on. FJ wins if in each of these pairs, his cow has the higher score.

Please help FJ count the number of different ways he and FP can choose their teams such that FJ will win the contest. That is, each distinct pair (set of $K$ cows for FJ, set of $K$ cows for FP) where FJ wins should be counted. Print your answer modulo 1,000,000,009.


## �����ʽ
The first line of input contains $N$, $M$, and $K$. The value of $K$ will be no larger than $N$ or $M$.

The next line contains the $N$ scores of FJ's cows.

The final line contains the $M$ scores of FP's cows.


## �����ʽ
Print the number of ways FJ and FP can pick teams such that FJ wins, modulo 1,000,000,009.


## ��Ŀ����
### ��Ŀ����

ÿ�꣬Farmer John ����������� $N$ ͷ��ţ�μ���չ����ġ����չʾ�����������ľ��� Farmer Paul Ҳ��������� $M$ ͷ��ţ�μӱ�����$1 \leq N \leq 1000, 1 \leq M \leq 1000$����

�μӱ�����ÿͷ $N + M$ ͷ��ţ������һ�������������÷֡�Ȼ������������ձ������� $K$ ͷ��ţ��ɵ��ŶӾ�����$1 \leq K \leq 10$�����������£�Farmer John �� Farmer Paul ����ѡ�� $K$ ͷ��ţ����Ŷӽ��б������������Ŷӵ���ţ�����÷ָߵ���ԣ�FJ �Ŷ��е÷���ߵ���ţ�� FP �Ŷ��е÷���ߵ���ţ��ԣ�FJ �Ŷ��е÷ֵڶ��ߵ���ţ�� FP �Ŷ��е÷ֵڶ��ߵ���ţ��ԣ��������ơ������ÿһ���У�FJ ����ţ�÷ֶ����ߣ���ô FJ ��ʤ��

����� FJ �������� FP ����ѡ���ŶӵĲ�ͬ��ʽ��������ʹ�� FJ �ܹ�Ӯ�ñ�����Ҳ����˵��ÿ����ͬ�ģ�FJ �� $K$ ͷ��ţ���ϣ�FP �� $K$ ͷ��ţ���ϣ��ԣ�ֻҪ FJ ��ʤ����Ӧ�����롣�������� $1\,000\,000\,009$ ȡģ��

### �����ʽ

����ĵ�һ�а��� $N$��$M$ �� $K$��$K$ ��ֵ���ᳬ�� $N$ �� $M$��

�ڶ��а��� FJ �� $N$ ͷ��ţ�ĵ÷֡�

�����а��� FP �� $M$ ͷ��ţ�ĵ÷֡�

### �����ʽ

��� FJ �� FP ����ѡ���Ŷӵķ�ʽ������ʹ�� FJ ��ʤ������� $1\,000\,000\,009$ ȡģ��

```input1
10 10 3
1 2 2 6 6 7 8 9 14 17
1 3 8 10 10 16 16 18 19 19
```

```output1
382
```

