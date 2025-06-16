## ��Ŀ����
��һ���� $N$ ���� $M$ ���ߣ����б�Ȩ������ͼ��ͼ���رߡ����Ի�����ı�Ŵ� $0$ ��ʼ��

���� $N-1$ ���ߵı�ȨΪ $1$������ߵı�Ȩ�� $\ge \lceil \frac{N}{3} \rceil$ �� $\le N$��ͬʱ����������Ǳ�ȨΪ $1$ �ıߣ�����ͼ����һ������

������Ҫ����ÿ����һ�飬��ʹ�����ı�Ȩ�ܺ���С��

����С�ı�Ȩ�ܺ͡�

**���ѣ�**
- ������������һ���ߡ�
- ��������ѡһ���������
- ��ֻ��һ���ˡ�

## �����ʽ
��һ��Ϊ�������� $N,M$��

������ $M$ �У�һ���������� $x_i,y_i,w_i$����ʾ��һ���� $x_i$ �� $y_i$����ȨΪ $w_i$ �ıߡ�

## �����ʽ
����ÿ����һ�飬������С�ı�Ȩ�ܺ͡�

```input1
9 10
0 1 1
0 2 1
0 3 1
1 4 1
2 5 1
2 6 1
3 7 1
3 8 1
2 4 5
6 7 3

```

```output1
11

```

## ��ʾ
#### ��������
![](https://cdn.luogu.com.cn/upload/image_hosting/5ftpjk6m.png?x-oss-process=image/resize,m_lfit,h_1700,w_2250)

����·��Ϊ $4\to 1\to 0\to 2\to 5\to 2\to 6\to 7\to 3\to 8$����Ȩ��Ϊ $1+1+1+1+1+1+3+1+1=11$��

#### ������
**����ʹ��������ԡ�**
- Subtask 1��$4$ �֣�����֤ $N\le 6$��$M\le 10$��
- Subtask 2��$8$ �֣�����֤ $N\le 20$��$M\le 40$��
- Subtask 3��$8$ �֣�����֤ $N\le 5\times 10^3$��$M\le 10^5$��$w_i=1$ �� $\lceil\frac{N}{2}\rceil\le w_i\le N$��
- Subtask 4��$24$ �֣�����֤ $N\le 100$��$M\le 200$��
- Subtask 5��$8$ �֣�����֤ $N\le 500$��$M\le 10^3$��
- Subtask 6��$12$ �֣�����֤ $N\le 5\times 10^3$��$M\le 10^5$��
- Subtask 7��$20$ �֣�����֤ $N\le 8\times 10^4$��$M\le 1.6\times 10^5$��
- Subtask 8��$16$ �֣������������ơ�

���� $100\%$ �����ݣ���֤ $4\le N\le 5\times 10^5$��$N-1 \le M\le 2\times 10^6$��$0\le x_i,y_i\le N-1$��$w_i=1$ ���� $\lceil \frac{N}{3}\rceil\le w_i\le N$��

#### ˵��
�������� [Canadian Computing Olympiad 2020](https://cemc.math.uwaterloo.ca/contests/computing/2020/index.html) [Day 1](https://cemc.math.uwaterloo.ca/contests/computing/2020/cco/day1.pdf) T3 Mountains and Valleys��

��Ϊ�������ݵ�϶ࣨ$119$ ���������Ա�����Ե���ɾ����

