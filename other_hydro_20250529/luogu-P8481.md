## ��Ŀ����
$\text{bh1234666}$ ����ѧϰ[���ֲ���](https://baike.baidu.com/item/%E4%BA%8C%E5%88%86%E6%9F%A5%E6%89%BE/10628618?fr=aladdin)��

## ��Ŀ����
������֪���ֲ��ҵ� $\text{mid}$ �ڼ���ʱ����ȡ $\lfloor\dfrac{l+r}{2}\rfloor$ ���� $\lceil\dfrac{l+r}{2}\rceil$��������ѡ������֢�� $\text{bh1234666}$ ͬѧ���Լ��Ķ��ֲ��Ҵ����м������������ÿ�����ѡȡ���е�һ����Ϊ $\textit{mid}$��

ע�⣬ѡȡ��ͬ�� mid ��������Ҳ���ܵ�Ӱ�죬���Դ���Ϊ׼��

���� $\text{bh1234666}$ �����˶��ֲ���ʹ�õ����У���֤Ϊ�����������Լ�����ҪѰ�ҵ�������֤�������ڣ�������֪����������õ������ѭ����Ҫ���м��Σ��������� $\textit{cnt}$ �Ŀ��ܵ�����ֵ����Сֵ����

ѭ����
```cpp
int find(int *num,int x,int len)
{
	int l=0,r=len-1,mid,cnt=0,w;
	while(l<r)
	{
		cnt++;
		w=rand()%2;
		mid=(l+r+w)/2;
		if(num[mid]-w<x) l=mid+!w;
		else r=mid-w;
	}
	return mid;
}
```
�ݹ飺
```
int cnt;
int get(int *num,int x,int l,int r)
{
	if(l==r) return l;
	cnt++;
	int w=rand()%2;
	int mid=(l+r+w)/2;
	if(num[mid]-w<x) return get(num,x,mid+!w,r);
	else return get(num,x,l,mid-w);
}
int find(int *num,int x,int len)
{
	cnt=0;
	return get(num,x,0,len-1);
}
```
ע��������������ȫ�ȼۡ�

�ڴ˶����������е� $w$ ����������һ�����͡�

����������� $[0,7]$���� $8$ ����Ա����Ȼ $mid$ ��ȡֵ����Ϊ $w$ ��ȡֵ�ı���ı䣬��������ȷ��������һ���� $[0,3]$ �� $[4,7]$��ѡ�ֿ��Ծ�������������ģ�⡣

�������� $[0,6]$���� $7$ ����Ա��$\textit{mid}$ ��ȡֵ�� $w$ ��ȡֵ�޹أ����� $l$ �� $r$ ��ȡֵ���ܵ� $w$ ��Ӱ�죬����ȷ������������� $[0,2]$��$[3,6]$��$w=1$���� $[0,3]$��$[4,6]$��$w=0$����

## �����ʽ
��һ�и���һ������ $n$ ��ʾ���г��ȡ�

�ڶ��и������������� $n$ ��������ʾ $\text{bh1234666}$ �����С�

������һ������ $q$ ��ʾѯ�ʵĴ�����

������ $q$ ��ÿ��һ��������ʾ��Ҫ��ѯ�����֡�

## �����ʽ
����ÿ��ѯ�ʻش�һ����������ʾ��С��ѭ��������

```input1
10
1 2 4 6 7 8 10 13 15 17
3
4
10
15
```

```output1
3
3
3
```

```input2
13
1 2 4 6 10 12 19 23 45 99 101 123 134
5
1
2
10
19
123

```

```output2
3
4
3
3
4
```

## ��ʾ
### ���� 1 ����

�� $4$��

ȡ $[1,5]$��

ȡ $[1,3]$��

ȡ $[3,3]$���˳�ѭ������

### ���� 2 ����

��ѯ $10$ ��λ�á�

$$
[1,13] \stackrel{w=0}{\longrightarrow} [1,7]\stackrel{w=0}{\longrightarrow}[5,7] \stackrel{w=1}{\longrightarrow} [5,5]
$$

### ���ݷ�Χ��Լ��
�������**�������**������ $3$ �� $\text{subtask}$�����շ���Ϊ���� $\text{subtask}$ ����֮�͡�

$$
\def\arraystretch{1.5}
\begin{array}{|c|c|c|}\hline
\textbf{Task} & \textbf{Score} & \text{��������} \cr\hline
1 & 25 & n \le 20 \cr\hline
2 & 35 & n=2^k(k \in \mathbf{N}) \cr\hline
3 & 40 &  \cr\hline
\end{array}
$$

���� $100\%$ �����ݣ���֤ $1 \le n \le 2^{20}$��$1 \le q \le 100$��$1 \le num_i \le 10^9$��

������ [extra sub](https://www.luogu.com.cn/problem/P8487)��

