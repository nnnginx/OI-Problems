


## ��Ŀ����
��һ�ô�СΪ(n<=100000)������ÿ������Ȩֵvi��Ҫ��֧�����²�����
�����ӡ�������ĳ��ȡmax/min�����ӡ�����ĳ��ȡmax/min�������޸ġ����޸ġ���Ȩֵ��ת��������͡�����͡������10^9+7ȡģ�ķǸ�������ɡ�
���и�Ϊ1����֤�����е���Ȩֵ��ת������iΪj�����ȡ�
## �����ʽ
�����һ��һ��������n���ڶ���n������v�������е���n+1��ÿ��������u��v����u��v֮����һ���ߡ�
������һ��һ������(m<=100000)������m��ÿ��һ��������������ʽ���£�
SUBADD i v i����������v
SUBMAX i v i��������vȡmax
SUBMIN i v i��������vȡmin
CHAINADD i j v i��j��·����ÿ�������v
CHAINMAX i j v i��j��·����ÿ�����vȡmax
CHAINMIN i j v i��j��·����ÿ�����vȡmin
SUBXGW i v i�������޸�Ϊv
CHAINXGW i j v i��j��·����ÿ�����޸�Ϊv
CHAINREV i j i��j��·������Ȩֵ��ת
SUBQUE i ���i��������
CHAINQUE i j ���i��j·���ϵ�Ȩֵ��
����������v�͵�ĳ�ʼȨֵv����v<=1000000����֤ȫ�̲����е�Ȩֵ����10^9+7
## �����ʽ
����ÿ����Ͳ������һ�д����ӦȨֵ�͡�

```input1
10
-3 -2 1 3 1 -2 0 -5 1 4 
2 1
3 1
4 1
5 2
6 4
7 3
8 2
9 3
10 2
19
SUBADD 4 2
SUBXGW 9 -5
CHAINQUE 1 1
SUBQUE 9
SUBMAX 7 -1
SUBMIN 10 2
CHAINQUE 6 9
SUBQUE 1
CHAINADD 9 3 4
CHAINXGW 5 7 5
CHAINQUE 7 7
SUBQUE 1
CHAINMAX 8 7 -5
CHAINMIN 5 3 4
CHAINQUE 3 1
SUBQUE 5
CHAINREV 1 7
CHAINQUE 3 2
SUBQUE 7

```
```output1
1000000004
1000000002
1000000005
1000000001
5
26
8
4
13
4
```

## ��ʾ
û��д����ʾ
## ��Ŀ��Դ
By DpDarkFantasy


