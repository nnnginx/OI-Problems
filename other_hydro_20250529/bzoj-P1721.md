## ��Ŀ����
Farmer Ron in Colorado is building a ski resort for his cows (though budget constraints dictate construction of just one ski lift). The lift will be constructed as a monorail and will connect a concrete support at the starting location to the support at the ending location via some number of intermediate supports, each of height 0 above its land. A straight-line segment of steel connects every pair of adjacent supports. For obvious reasons, each section of straight steel must lie above the ground at all points. Always frugal, FR wants to minimize the number of supports that he must build. He has surveyed the $n \ (2  \leq  n  \leq  5\times 10^3)$ equal-sized plots of land the lift will traverse and recorded the integral height $h \ (0  \leq  h  \leq  10^9)$ of each plot. Safety regulations require FR to build adjacent supports no more than $k \ (1  \leq  k  \leq  n - 1)$ units apart. The steel between each pair of supports is rigid and forms a straight line from one support to the next. Help FR compute the smallest number of supports required such that: each segment of steel lies entirely above (or just tangent to) each piece of ground, no two consecutive supports are more than $k$ units apart horizontally, and a support resides both on the first plot of land and on the last plot of land.

�������ݵ��޶�����Ϊ������ţ�ǽ���һ����ѩ������Ȼ��Ҫ����ʩ������һ���³�������һ���³�����Ҫ��ɽ�ŵ�ɽ�������ɸ����ӣ����ø�˿�������ǡ��������Ϊ����ڵ��棬���ӵĸ߶ȿ��Ժ��Բ��ơ�ÿ�����������Ӽ䶼�и�˿ֱ����������Ȼ�����и�˿���κ�һ�ζ������ڵ���֮�¡�Ϊ�˽�ʡ����ķ��ã��޶�ϣ���ڹ������޽��������ٵ����ӡ�����׼���޽��³���ɽ���ϵ����� $n$ ������֮��ˮƽ������ȵĵ㣬���Ҳ�����ÿ����ĸ߶� $h$�����ң����չ��Ұ�ȫ��׼�������������Ӽ�ľ��벻�ܳ��� $k$ ����λ���ȡ����Ӽ�ĸ�˿���Ǳ�ֱ��. �޶�ϣ�����������һ�£���������������������£�������Ҫ�޽����ٸ����ӣ����ȣ����е����Ӷ������޽�������ѡ���ĵ��ϣ���ÿһ�θ�˿��������ڵ���������ø��������С������������ӵľ��벻���� $k$ ����λ���ȡ���Ȼ���ڵ�һ���������һ������һ����Ҫ�޽����ӡ�
## �����ʽ

�� $1$ �У��������� $n$ �� $k$���ÿո������

�� $2$ �� $n+1$ �У�ÿ�а���һ������������ $i+1$ �е��������˵� $i$ ����ĸ߶ȡ�

## �����ʽ

���һ�����������޶�������Ҫ�޽������ӵ���Ŀ��

```inout1
13 4
0
1
0
2
4
6
8
6
8
8
9
11
12
```
```output1
5
```
## ����˵��

�޶�����Ҫ�޽� $5$ �����ӣ��ֱ��ڵ� $1,5,7,9,13$ ��ɽ���ϵĵ㣩����˿�� $1-5,5-7,7-9$ �Լ� $12-13$ �� $4$ ������������С�
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$2 \leq n \leq 5\times 10^3$��$0 \leq h \leq 10^9$��$1 \leq k \leq n-1$��
## ��Ŀ��Դ
Gold