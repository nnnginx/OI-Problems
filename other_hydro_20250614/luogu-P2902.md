## ��Ŀ����
At Bessie's recent birthday party, she received $N(2 \le N \le 10^5,N\equiv0\pmod{2})$ pearls, each painted one of C different colors ($1\le C \le N$).

Upon observing that the number of pearls $N$ is always even, her creative juices flowed and she decided to pair the pearls so that each pair of pearls has two different colors.

Knowing that such a set of pairings is always possible for the supplied testcases, help Bessie perform such a pairing. If there are multiple ways of creating a pairing, any solution suffices.

�� Bessie ��������վۻ��ϣ����յ� $N(2\le N \le 10^5,N\equiv0\pmod{2})$ �����顣һ���� $C$ ����ɫ�����飨$1\le C \le N$������ $i$ ����ɫ�������� $C_i$ �š�


�۲쵽��������� $N$ ����ż�������Ĵ������ˣ�����������飬ʹÿ�����������ֲ�ͬ����ɫ�����ݱ�֤���ڴ𰸡������ Bessie ִ����������ԣ�����ж�����Եķ������������һ�ּ��ɡ�

## �����ʽ
Line $1$: Two space-separated integers: $N$ and $C$.

Lines $2 \ldots C+1$: Line $i+1$ tells the count of pearls with color $i$: $C_i$.

�� $1$ �У������ո�ָ���������$N$ �� $C$��

�� $2\ldots C+1$�У��� $i+1$ Ϊ��ɫ $i$ �������� $C_i$��

## �����ʽ
Lines $1\ldots \dfrac{N}{2}$: Line $i$ contains two integers $a_i$ and $b_i$ indicating that Bessie can pair two pearls with respective colors $a_i$ and $b_i$.

�� $1\ldots \dfrac{N}{2}$ �У��� $i$ �а����������� $a_i$ �� $b_i$����ʾ Bessie ���Խ�������ɫΪ $a_i$ �� $b_i$ ������������ԡ�

```input1
8 3 
2 
2 
4 

```

```output1
1 3 
1 3 
2 3 
3 2 

```

## ��ʾ
There are $8$ pearls and $3$ different colors. Two pearls have color $\mathrm{I}$; two have color $\mathrm{II}$; four have color $\mathrm{III}$.


Bessie pairs each pearl of color $\mathrm{III}$ with one of color $\mathrm{I}$ and $\mathrm{Ii}$.

˵������ $8$ ������� $3$ �ֲ�ͬ����ɫ������������ɫΪ $1$������������ɫΪ $2$���Ŀ�������ɫΪ $3$��

Bessie ��ÿ����ɫΪ $3$ ����������ɫΪ $1$ �� $2$ ��������ԡ�

��л@[�߶�ľ](https://www.luogu.com.cn/user/33930) �ṩ���룬@[PineappleSummer](https://www.luogu.com.cn/user/880187) ���������Լ��ṩ $\LaTeX$��

