## ��Ŀ����
Farmer John wants to take Bessie skiing in Colorado. Sadly, Bessie is not really a very good skier.

Bessie has learned that the ski resort is offering S (0 <= S <= 100) ski classes throughout the day. Lesson i starts at time M\_i (1 <= M\_i <= 10,000) and lasts for time L\_i (1 <= L\_i <= 10,000). After lesson i, Bessie's ski ability becomes A\_i (1 <= A\_i <= 100). Note: this ability is an absolute, not an incremental change.

Bessie has purchased a map which shows all N (1 <= N <= 10,000) ski slopes along with the time D\_i (1 <= D\_i <= 10,000) required to ski down slope i and the skill level C\_i (1 <= C\_i <= 100) required to get down the slope safely. Bessie's skill level must be greater than or equal to the skill level of the slope in order for her to ski down it.

Bessie can devote her time to skiing, taking lessons, or sipping hot cocoa but must leave the ski resort by time T (1 <= T <= 10,000), and that means she must complete the descent of her last slope without exceeding that time limit.

Find the maximum number of runs Bessie can complete within the time limit. She starts the day at skill level 1.

Extra feedback will be provided on the first 50 submissions.



## �����ʽ
\* Line 1: Three space-separated integers: T, S, and N

\* Lines 2..S+1: Line i+1 describes ski lesson i with three

space-separated integers: M\_i, L\_i, and A\_i

\* Lines S+2..S+N+1: Line S+i+1 describes ski slope i with two

space-separated integers: C\_i and D\_i.


## �����ʽ
A single integer on a line by itself, the maximum number of runs that Bessie may ski within the time limit.


## ��Ŀ����
Farmer John ��Ҫ���� Bessie һ���ڿ���������һ��ѩ���ܲ��ң�Bessie ��ѩ����������տ��Bessie�˽⵽���ڻ�ѩ���ÿ����ṩ $S(0 \le S \le 100)$ �Ż�ѩ�Ρ��� $i$ �ڿ�ʼ�� $M_i(1 \le M_i \le 10000)$ �ϵ�ʱ��Ϊ $L_i(1 \le L_i \le 10000)$��

����� $i$ �ڿκ�Bessie �Ļ�ѩ�������� $A_i(1 \le A_i \le 100)$. ע�⣺��������Ǿ��Եģ���������������ֵ��

Bessie ����һ�ŵ�ͼ����ͼ����ʾ�� $N(1 \le N \le 10,000)$ ���ɹ���ѩ��б�£��ӵ�i��б�µĶ��˻����ײ������ʱ�� $D_i(1 \le D_i \le 10000)$���Լ�ÿ��б������Ҫ�Ļ�ѩ���� $C_i(1 \le C_i \le 100)$���Ա�֤��ѩ�İ�ȫ�ԡ�Bessie ������������ڵ�������ȼ�����ʹ�����ܹ���ȫ���¡�

Bessie ����������ʱ������ѩ���ϿΣ����������غ���һ���ɿ�֭�������������� $T(1 \le T \le 10000)$ ʱ���뿪��ѩ��������ζ���������� $T$ ʱ��֮ǰ������һ�λ�ѩ�� �� Bessie ��ʵ������������ɶ��ٴλ�ѩ����һ�쿪ʼ��ʱ�����Ļ�ѩ����Ϊ $1$.


```input1
10 1 2 
3 2 5 
4 1 
1 3 

```

```output1
6 

```

## ��ʾ
Ski the second slope once, take the lesson, and ski the first slope 5 times before time is up: a total of 6 slopes.


