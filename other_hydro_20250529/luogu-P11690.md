## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/ivkgc3xh.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/h5h2nanp.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/c2ur90co.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/bv38t9mw.png)

## ��Ŀ����
> ���������������޻ڡ�����˼��������Զ����



����һ�� $n$ ������������ $i$ ������� $b_i$ �����ӣ�������ܷ� $a_i$ �����ӡ�������һ����� $k$ �Ǹ���ÿ�β��������ѡ��һ����㣬������һ�����ӣ��Ƶ����ĸ����ϣ���Ҫ���������׵�������û�г������ƣ�Ȼ����Ҫ��С���������ӵ� $k$ �ľ���͡�

�� $k = 1, 2, \cdots, n$ ������𰸡�

## �����ʽ
��һ�а���һ�������� $n$ ��ʾ���Ľ��������

�ڶ��а��� $n$ ������������ $i$ ����������ʾ�� $i$ �����������ܷ� $a_i$ �����ӡ�

�����а��� $n$ ������������ $i$ ����������ʾ�� $i$ ������ϳ�ʼ���� $b_i$ �����ӡ�

������ $n-1$ �У�ÿ�������� $u,v$����ʾ���ϵ�һ���ߡ�


## �����ʽ
һ�� $n$ ���������� $i$ ��������ʾ $i$ ��Ϊ��ʱ�Ĵ𰸡�

```input1
3
6 2 10 
6 0 2 
1 2
2 3
```

```output1
2 6 0
```

```input2
5
7 6 2 1 10 
3 5 0 0 7 
1 2
2 3
1 4
4 5
```

```output2
10 12 20 14 9
```

## ��ʾ
Idea��zhaohaikun��Solution��zhaohaikun��Code��zhaohaikun��Data��zhaohaikun��

���������������㣺$1\le n\le 5\times 10^5$��$0 \le b_i \le a_i$��$1\le a_i\le 10^7$��Ϊ�˱���𰸱� long long���� $a_i$ �ķ�Χ��С��һ�㡣

subtask 1��$1$ �֣���$b_i=0$��

subtask 2��$5$ �֣���$n\le 2000$��

subtask 3��$11$ �֣���$n\le 8000$��

subtask 4��$3$ �֣���������֤ $\forall i\in [1, n-1]\cap \mathbb{Z}$������ $i$ �� $i+1$ �бߣ�

subtask 5��$3$ �֣����ջ�����֤ $\forall i\in [2, n]\cap \mathbb{Z}$������ $1$ �� $i$ �бߣ�

subtask 6��$6$ �֣�����֤�������

subtask 7��$16$ �֣���$a_i\le 5$��

subtask 8��$22$ �֣���$n\le 5\times 10^4$��

subtask 9��$16$ �֣���$n\le 10^5$��

subtask 10��$11$ �֣���$n\le 2\times 10^5$��

subtask 11��$5$ �֣���$n\le 3\times 10^5$��

subtask 12��$1$ �֣����ޡ�

����˵������������ɷ�ʽ�����ڽ�� $i\in [2,n]$���� $[1,i-1]$ �ڵȸ������һ���� $p$���� $i,p$ ��һ���ߡ�

