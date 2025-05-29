## ��Ŀ����
> ����ϵ�Ľ��ۻ�������Ͳ���ˮƽ���Ļ�е�Ƶ������������Ŀ����Ҫ���߲���ˮƽ������С�

����command_block ����ǰС��ʿ��

[](https://cdn.luogu.com.cn/upload/image_hosting/1m9hce9x.png)����ѡ�ֳ�˼ά�⡣

## ��Ŀ����
��Ҫ�� djy ��һ��������������������

- �� $n$ ������ɡ�

- $i$ �ŵ�Ķ���Ϊ $a_i$��

����һ���� $(i,j)$ �ļ�ֵΪ $b_i\times b_j$����Ҫ�������������������£�ʹ���бߵļ�ֵ�����

��֤��������������

## �����ʽ
��һ��һ������ $type$����ʾ�������ɷ�ʽ��

�� $type=0$��

�ڶ���һ������ $n$��

������ $n$ ���������� $i$ ������ʾ $a_i$��

������ $n$ ���������� $i$ ������ʾ $b_i$��

�� $type=1$��

����һ������������ģ�壺

```cpp
int a[10000005],b[10000005];
unsigned seed;
unsigned rnd(unsigned x){
	x^=x<<13;
	x^=x>>17;
	x^=x<<5;
	return x;
}
int rad(int x,int y){
	seed=rnd(seed);
	return seed%(y-x+1)+x;
}
void init_data(){
	cin>>seed;
	for(int i=1;i<=n;i++)
		a[i]=1,b[i]=rad(1,500000);
	for(int i=1;i<=n-2;i++)
		a[rad(1,n)]++;
}
```

�ڶ���һ������ $n$��

֮����� `init_data()`��

������һ������ $seed$��

## �����ʽ
һ��һ������ $ans$����ʾ���ļ�ֵ�͡�

```input1
0
5
1 2 3 1 1 
5 3 1 7 9
```

```output1
42
```

```input2
1
10
114514
```

```output2
249899101316
```

## ��ʾ
**�������������ԡ�**

- Subtask0 (10 pts)��$n\le 6$��$type=0$��
- Subtask1 (20 pts)��$n\le 10^3$��$type=0$��
- Subtask2 (10 pts)��$n\le5\times10^5$��$b_i\le2$��$type=0$��
- Subtask3 (20 pts)��$n\le10^5$��$type=0$��
- Subtask4 (20 pts)��$n\le5\times10^5$��$type=0$��
- Subtask5 (20 pts)��$type=1$��

���� $100\%$ �����ݣ�$2\le n\le10^7$��$1\le a_i\le n$��$1\le b_i\le5\times10^5$��$type\in\{0,1\}$��$0\le seed<2^{31}$��

