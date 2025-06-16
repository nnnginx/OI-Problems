## ��Ŀ����
After several months of rehearsal, the cows are just about ready to put on their annual dance performance; this year they are performing the famous bovine ballet "Cowpelia".

The only aspect of the show that remains to be determined is the size of the stage. A stage of size $K$ can support $K$ cows dancing simultaneously. The $N$ cows in the herd ($1 \leq N \leq 10,000$) are conveniently numbered $1 \ldots N$ in the order in which they must appear in the dance. Each cow $i$ plans to dance for a specific duration of time $d(i)$. Initially, cows $1 \ldots K$ appear on stage and start dancing. When the first of these cows completes her part, she leaves the stage and cow $K+1$ immediately starts dancing, and so on, so there are always $K$ cows dancing (until the end of the show, when we start to run out of cows). The show ends when the last cow completes her dancing part, at time $T$.

Clearly, the larger the value of $K$, the smaller the value of $T$. Since the show cannot last too long, you are given as input an upper bound $T_{max}$ specifying the largest possible value of $T$. Subject to this constraint, please determine the smallest possible value of $K$.



## �����ʽ
The first line of input contains $N$ and $T_{max}$, where $T_{max}$ is an integer of value at most 1 million.

The next $N$ lines give the durations $d(1) \ldots d(N)$ of the dancing parts for cows $1 \ldots N$. Each $d(i)$ value is an integer in the range $1 \ldots 100,000$.

It is guaranteed that if $K=N$, the show will finish in time.



## �����ʽ
Print out the smallest possible value of $K$ such that the dance performance will take no more than $T_{max}$ units of time.



## ��Ŀ����
### ��Ŀ����

���������µ���������ţ�ǻ���׼����չ�����ǵ�����赸���ݡ���������Ҫ���ݵ�����������ţ���١�����cowpelia����

����Ψһ�д�����������̨�ĳߴ硣һ����СΪ $K$ ����̨����֧�� $K$ ͷţͬʱ����̨�����衣��ţȺ�е� $N$ ͷţ�������Ǳ���������赸�е�˳�򷽱�ر��Ϊ $1,2,\dots,N$���� $i$ ͷţ�ƻ��� $d_i$ ���ض�����ʱ�䡣
һ��ʼ���� $1,2,\dots,K$ ͷţ��������̨�ϲ���ʼ���衣����Щţ�е�ĳһͷţ������������Ĳ��֣����������뿪��̨���ҵ� $K+1$ ͷţ���������̨�ϲ���ʼ���衣���ԣ���̨������ $K$ ͷ��ţ�����裨ֱ�����ݵ�β������ţ������ʱ�򣩡������һͷ��ţ����������赸���֣����ݽ����������� $T$ ����λʱ�䡣

��Ȼ��$K$ ��ֵԽ��$T$ ��ԽС�����ڱ��ݲ�����̫�������֪��ָ�� $T$ ��������ֵ������ $T_{max}$����������Լ����ȷ�� $K$ ����Сֵ��

### �����ʽ

��һ�а��� $N$ �� $T_{max}$ ����������

�������� $N$ �У��� $i$ �и����˵� $i$ ͷţ����ĳ���ʱ�� $d_i$���� $i$ �а���һ������ $d_i$��

��֤ $K=N$ ʱ���ݻᰴʱ��ɡ�

### �����ʽ

����ڱ���ʱ�䲻���� $T_{max}$ ʱ�� $K$ ����С����ֵ��

### ��ʾ˵��

���� $100\%$ �����ݣ�$1 \le N \le 10^4$��$T_{max} \le 10^6$��$1 \le d_i \le 10^5$��

```input1
5 8
4
7
8
6
4
```

```output1
4

```

