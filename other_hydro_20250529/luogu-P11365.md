## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/pcokv5zr.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/hasy3fee.png)

## ��Ŀ����
�������� $a_1,\dots,a_n$���� $m$ ��ѯ�ʣ��� $i$ ��ѯ�ʸ��� $m_i$ ������ $[l_j,r_j],\;1\le j\le m_i$������ $1\le l_j\le r_j\le n,\;r_j<l_{j+1}$������Ҫ����м�����Ԫ�� $(p,q)$ ���� $p<q,\;a_p<a_q$���Ҵ��� $1\le u<v\le m_i$ ʹ�� $l_u\le p\le r_u,\;l_v\le q\le r_v$��

## �����ʽ
��һ����������ʾ $n,m$��

������һ�� $n$ ������ʾ $a_1,\dots,a_n$��

��������ÿ��ѯ�ʵ�һ��Ϊ $m_i$�������� $m_i$ ��Ϊ $l_j,r_j$��

## �����ʽ
�� $m$ �У�����Ϊÿ��ѯ�ʵĴ𰸡�

```input1
5 2
5 4 2 3 1
3
1 1
2 3
4 4
2
1 2
3 4
```

```output1
1
0
```

## ��ʾ
Idea��nzhtl1477��Solution��ccz181078��Code��ccz181078��Data��ccz181078

���� $100\%$ �����ݣ����� $1\le n\le 5\times 10^5$��$1\le \sum\limits_{i=1}^m m_i\le 5\times 10^5$��$m_i\ge 1$��$1\le a_i\le n$��������ֵΪ������

���� $0\%$ �����ݣ����� $n\le 10^3,\;\sum\limits_{i=1}^m m_i\le 10^3$��

�������� $10\%$ �����ݣ����� $m_i\le 10$��

�������� $10\%$ �����ݣ����� $m\le 5$��

�������� $80\%$ �����ݣ����������ơ�

