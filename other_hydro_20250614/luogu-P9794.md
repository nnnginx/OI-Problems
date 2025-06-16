## ��Ŀ����
������ [NERC 2018](https://neerc.ifmo.ru/archive/2018/neerc-2018-statement.pdf) D �⡣

## ��Ŀ����
����һ�� $n$ ������ $m$ ���ߵ���ͨ����ͼ������ $u$ �� $v$ �ľ��� $d(u, v)$ Ϊ�� $u$ �� $v$ ���·���Ͼ����ı�����

����������� $\sum_{u=1}^n \sum_{v=u+1}^n d(u,v)$��

## �����ʽ
��һ�и����������� $n(1 \leq n \leq 10^5)$��$m(n - 1 \leq m \leq n + 42)$���ֱ��ʾ�����ͱ�����

������ $m$ �У�ÿ�� $2$ ������ $x_i$ �� $y_i(1 \leq x_i,y_i \leq n, x_i \neq y_i)$����ʾ $x_i$ �� $y_i$ ֮����һ���ߡ�

��֤û���رߺ��Ի���

## �����ʽ
��� $\sum_{u=1}^n \sum_{v=u+1}^n d(u,v)$��

```input1
4 4
1 2
2 3
3 1
3 4
```

```output1
8
```

```input2
7 10
1 2
2 6
5 3
5 4
5 7
3 6
1 7
5 1
7 4
4 1
```

```output2
34
```

## ��ʾ
�����������ݱ�֤ $1 \leq n \leq 10^5$��$n-1 \leq m \leq n + 42$��$1 \leq x_i, y_i \leq n$ �� $x_i \neq y_i$��

����һ��ͼ�ǣ�

![](https://cdn.luogu.com.cn/upload/image_hosting/39wue8qr.png)

���� $d(1,2) = 1$��$d(1,3) = 1$��$d(1,4) = 2$��$d(2,3) = 1$��$d(2,3) = 2$��$d(3,4) = 1$���ܺ�Ϊ $1 + 1 + 2 + 1 + 2 + 1 = 8$��

������Ϊ��

![](https://cdn.luogu.com.cn/upload/image_hosting/89k279bd.png)

