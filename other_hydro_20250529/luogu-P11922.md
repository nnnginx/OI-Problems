## ��Ŀ����
PA 2025 R4C.



## ��Ŀ����

�� $n$ ���������ľ����� $1\sim a_i$���� $i$ ���ľ�ı߳�Ϊ $a_i$��ͼ������Ϊ $w_i$��

���ǳ�һ��**��**��һ������ $p_1,p_2,\ldots,p_m$������ $1\le p_i\le n$���� $p_i$ ������ͬ��

һ������**�ȵ�**�����ҽ�����

- $\forall 1\le i\lt m$��$a_{p_i}\gt a_{p_{i+1}}$��

���������� $c$������һ������**���۶�**Ϊ��

$$\sum_{1\le i\le m} a_{p_i}-c\cdot \sum_{1\le i\lt m} [w_{p_i}\neq w_{p_{i+1}}]$$

���仰˵����������Ļ�ľ�߶ȼ�ȥ�����ڵĲ�ͬͼ���Ļ�ľ�������� $c$����

���**�ȵ�**����������۶ȡ�


## �����ʽ
��һ�У������� $n,c$��

������ $n$ �У��� $i$ ������������ $a_i,w_i$��

��֤ $\forall 1\le i\lt n$���� $a_i\le a_{i+1}$��


## �����ʽ
���һ��һ����������ʾ�ȵ�����������۶ȡ�


```input1
4 1
1 1
3 2
4 3
4 1
```

```output1
6
```

```input2
4 5
1 1
3 2
4 3
4 1
```

```output2
5
```

## ��ʾ
### ��������

**����������**���Ŀ��ľ����״��ͼ��������ʾ����������Ψһ������ֻ�� $c$��

![](https://cdn.luogu.com.cn/upload/image_hosting/fgnbuet8.png?x-oss-process=image/resize,m_lfit,h_150)


���� $1$ �У���ͼ�������ȵ��������۶������ģ�Ϊ $4+3+1-(1+1)\times 1=6$��

![](https://cdn.luogu.com.cn/upload/image_hosting/ys9t7rao.png?x-oss-process=image/resize,m_lfit,h_150)


���������� $2$ �У���ͼ���������۶�Ϊ $-2$������ $2$ �����۶������ȵ���������ʾ���������۶�Ϊ $4+1-5\times 0=5$��

![](https://cdn.luogu.com.cn/upload/image_hosting/l1ou8e1y.png?x-oss-process=image/resize,m_lfit,h_100)

### ������

�ڼ�ֵ $50$ �ֵ��������У����� $\forall 1\le i\lt n$��$a_i\lt a_{i+1}$��

### ���ݷ�Χ

- $1\le n,c,a_i,w_i\le 5\times 10^5$��
- $\forall 1\le i\lt n$��$a_i\le a_{i+1}$��


