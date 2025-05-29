## ��Ŀ����
����һ������Ϊ $n$ ������ $\textbf A$��һ��ֵ��Ϊ $[1,n-1]$ �ĳ���Ϊ $n+1$ ������ $\textbf{ID}$ ��һ������ $r$��

����ͨ������α��������� $\textbf A$ ���� Warshall-Turing-Fourier �任 $^\textsf{[1]}$��

```cpp
sum = 0
for i = 1 to n
	index = min{ID[i], ID[i+1]}
	sum = sum + A[index]
	Rorate(A, r)
Change(A)
for i = 1 to n
	index = max{ID[i], ID[i+1]}
	index = index + 1
	sum = sum + A[index]
	Rorate(A, r)
```

���У�
- $\texttt{Change}(\textbf A)$ ��ʾ������ $\textbf A$ ������Ԫ�طֱ�ĳ����ǵ��෴����
- $\texttt{Rorate}(\textbf A,r)$ ��ʾ������ $\textbf A$ ��������õ����� $\textbf B$��ȡ $\textbf B[n-r+1,2n-r]$ �������� $\textbf A$��\
  ��**������ת** $R$ ��λ�á�

���Ѿ�֪������ $\textbf A$ ������ $r$�����㲢��֪������ $\textbf{ID}$��

����Ҫ��� WTF �任��α������ $\text{sum}$ ���ܵ����ֵ��

$\textsf{[1]}$��ʵ���ϲ������ڣ���ȻҲ���Խ�����Sept �任����

## �����ʽ
��һ���������� $n,r$��

������һ�� $n$ ����������ʾ���� $\textbf A$��

## �����ʽ
��һ��һ����������α������ $\text{sum}$ ���ܵ����ֵ��

�ڶ��� $n+1$ ����������ʹ�� $\text{sum}$ ֵ���� $\textbf{ID}$ ���顣

**������ڶ���⣬�������һ�֡�**

```input1
5 3
1 -1 1 -1 1
```

```output1
10
1 1 1 2 2 3
```

```input2
6 5
2 5 4 1 3 5
```

```output2
16
3 2 1 1 5 4 1
```

## ��ʾ
#### �зַ�ʽ

������ֻ�е�һ����ȷ�����Եõ� $50\%$ �ķ�����

**������뱣֤�ڶ����� $\bm{n+1}$ ������Ҫ�������**

#### ���ݹ�ģ��Լ��

**������� Special Judge��**

- ���� $20\%$ �����ݣ��� $n\le 7$��
- ���� $60\%$ �����ݣ��� $n\le 300$��
- ���� $100\%$ �����ݣ��� $2\le n\le 3\times 10^3$��$1\le r\le n$��$\textbf A[i]\in[-10^4,10^4]$��

����Ҫ��֤�㹹��� $\textbf{ID}[i]\in[1,n-1]$��

#### ˵��

��ԭ�����ã����� 160 �֡�

���� **[COCI 2014-2015](https://hsin.hr/coci/archive/2014_2015/)** [Contest #6](https://hsin.hr/coci/archive/2014_2015/contest6_tasks.pdf) Task F _**WTF**_��

