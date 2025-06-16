## ��Ŀ����
The aliens from outer space have (finally!) invaded Earth. Defend yourself, or be disintegrated!

Or assimilated. Or eaten. We are not yet sure.

The aliens follow a known attack pattern. There are $n$ attackers, the $i-th$ one appears at time $a_i$, at distance $d_i$ from you. He must be destroyed no later than at time $b_i$, or else he will fire his weapon, which will definitely end the fight.

Your weapon is an area-blaster, which can be set to any given power. If fired with power $R$,it momentarily destroys all aliens at distance $R$ or smaller. It also consumes $R$ fuel cells.

Determine the minimal cost (measured in fuel cells) of destroying all the aliens, without being killed.

## �����ʽ
The first line of input contains the number of test cases $T$. The descriptions of the test cases follow:

Each test case starts with a line containing the number of aliens $n(1 \le n \le 300)$. Of the next $n$ lines, the $i-th$ one contains three integers $a_i, b_i, d_i, (1 \le a_i < b_i \le 10 000, 1 \le d_i \le 10 000)$.

The $i-th$ alien appears at time $a_i$, is idle until $b_i$, and his distance from you is $d_i$.


## �����ʽ
For each test case, output one line containing the minimum number of cells needed to destroy all the aliens.


## ��Ŀ����
### ��Ŀ����
������̫�յ������ˣ����գ������˵��򡣱����Լ������߽��壬������ͬ�������߳�Ϊʳ�����Ϊֹ�������޷�ȷ����

��������ѭ��֪�Ĺ���ģʽ���� $N$ �������˽������� $i$ �������������˻���ʱ�� $a_i$ ���֣�������ľ���Ϊ $d_i$����������ʱ�� $b_i$ ǰ�����𣬷�������Ļ����㡣

���������һ�����������������������κθ����Ĺ��ʡ�����������˹��� $R$������˲��ݻ�����ľ����� $R$ ���ڵ����������ˣ����Ե��ڣ���ͬʱ��Ҳ������ $R$ ��λ��ȼ�ϵ�ء�

��ݻ����������˵���ͳɱ������Ķ���ȼ�ϵ�أ���ͬʱ��֤�Լ���������ȫ��

### �����ʽ

��һ������һ���� $T$,��ʾ�� $T$ �����ݡ�

ÿ�����ݵĵ�һ��Ϊ�����˵����� $n$��$1\leq n\leq 300$����

������ $n$ �У�ÿ���������� $a_i,b_i,d_i$����ʾ�����������ʱ�� $a_i$ ���֣������� $d_i$���� $b_i$ ǰʱ��������

### �����ʽ

�� $T$ �У�ÿ������ݻ����������˵���ͳɱ���

```input1
1
3
1 4 4
4 7 5
3 4 7

```

```output1
7
```

