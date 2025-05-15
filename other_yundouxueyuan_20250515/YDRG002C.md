## ��Ŀ����

![Snipaste\_2023-08-07\_20-25-01.png](https://img.macesuted.moe/43b8403457e60dc3a19d2e4ca0df975a/5fb1f8b2a75a7.png)

## ��Ŀ����

�������Ŀ�У�����Ҫ�������һ�����⣺

����һ������Ϊ $w$��$w=60$���� $01$ ���� $a_{0,1,2\dots,w-1}$������Ҫ������ж��ٸ������������͵������䳤�ȡ�

Ϊ��ѹ�������������� $a$ ����������ķ������ɣ�����ģ��㽫����һ�������� $x$��$x< 2^{w}$�� ��ʾ $a$������ $x=a_0\times 2^{0}+a_1\times 2^1\dots a_{w-1}\times 2^{w-1}$��

�����ж���ѯ�ʣ��� $q$��$q\le 5\times 10^7$�� �Σ������ö����������ϵķ�ʽ���ɣ����巽���������ʽ��

## �����ʽ

��һ���ĸ������� $q,k,a,c$������ $q$ �ĺ������Ŀ������$k,a,c$ ���Զ������ݣ����巽�����£�

�������� $q$ ��ѯ���У�ǰ $k$ ��ѯ�ʵ� $x_1,x_2,\dots,x_k$ �������и�����ÿ��һ�����ӵ� $k+1$ ��ѯ�ʿ�ʼ�� $x_i=(\operatorname{xorshift}(x_{i-1})+a)\bmod c$������ $\operatorname{xorshift}$ �ľ��庬�彫���·��Դ�����ʽ������

��֤ $c\leq 2^w$��

$\operatorname{xorshift}$ ����Ƭ�����£�

```cpp
unsigned long long xorshift(int X){
	X ^= X << 13; X ^= X >> 17; X ^= X << 5; return X;
}
```

����ģ�壬��֤�ö���ģ���ʱС�� $\text{600 ms}$��

```cpp
#include<bits/stdc++.h>
unsigned long long a, c, x;
int q, k;
namespace Read{
	int cnt = 0; unsigned long long X;
	unsigned long long read(){
		if(++ cnt <= k) {std :: cin >> X; return X;}
		else {X ^= X << 13; X ^= X >> 17; X ^= X << 5; return X = (X + a) % c;}
	}
}
int main(){
	std :: ios :: sync_with_stdio(false); std :: cin.tie(0);
	std :: cin >> q >> k >> a >> c; 
	for(int i = 1; i <= q; i ++){
		x = Read :: read();
		/*
			Write your code.
		*/
	}
}
```

## �����ʽ

Ϊ�˼�С��������ǵ� $i$ ��ѯ�ʵĴ�Ϊ $p_i$����ֻ��Ҫ��� $(1\times p_1)\oplus (2\times p_2)\oplus\dots (q\times p_q)$ ��ֵ������ $\oplus$ ��ʾ��������������

## ���� #1

### �������� #1

```
1 1 1 1
12345678910
```

### ������� #1

```
59
```

### ���ݷ�Χ��Լ��

�������������ԡ�

���� $100\%$ �����ݱ�֤ $k\le10^6, q\leq5\times 10^7$��

| ��������| $q=$ | $k\leq$ |����|
| :---: | :---: | :---: | :---: |
| $1$ | $5\times 10^6$ | $10^6$ |$30$|
| $2$ | $5\times 10^7$ | $10^6$ |$70$|

