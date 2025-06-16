## ��Ŀ����
��������ƣ�������������ɾ��������ȫ�������뵽 [InfOJ](http://119.27.163.117/contest/7/)��

## ��Ŀ����
��������Ϊ $n$ ������ $[a_1,a_2,\dots ,a_n]$��

$m$ ��ѯ�ʣ�ÿ�θ����ĸ������� $L_1,R_1,L_2,R_2\ (1\le L_1\le R_1\le 4000,1\le L_2\le R_2\le 4000)$�����ж��ٸ����� $[l,r]\ (1\le l\le r\le n)$ ���� $a_l,a_{l+1},\dots,a_r$ �е����ֵ���� $[L_1,R_1]$����Сֵ���� $[L_2,R_2]$��

ѯ�ʴ����ܴ�����ѯ�����ڳ��������ɵġ��������Ķ���ʾ˵��һ���Ĵ��롣

## �����ʽ
��һ������������ $n,m$��

������һ�� $n$ �������� $a_1\sim a_n$��

������һ������������ $p,q,seed$��Ϊ�����������Ĳ������㲻��Ҫ���������������������й��̣���ֻ��Ҫ֪���������ȷ������ѯ�ʵĻ���һ���� $L_1,R_1,L_2,R_2\in [p,q]$��

## �����ʽ
��� $i$ ��ѯ�ʵĴ�Ϊ $ans_i$�����һ��һ��������Ϊ $\operatorname{xor}_{i=1}^m 
(i\times ans_i)$ ��ֵ��

```input1
5 5
2 4 1 3 5
1 5 1145141919810
```

```output1
24
```

```input2
10 20000000
1 3 4 10 5 5 2 7 10 7
1 10 23333333333333333
```

```output2
548722417
```

## ��ʾ
**���� 1 ����**

���ѯ�ʵ� $(L_1,R_1,L_2,R_2)$ �ֱ�Ϊ $(1,5,1,5),(1,2,2,4),(3,4,2,2),(2,4,2,2),(2,5,2,5)$���𰸷ֱ�Ϊ $15,1,1,2,6$��

��� $(1\times 15)\ \mathrm{xor}\ (2\times 1)\ \mathrm{xor}\ (3\times 1)\ \mathrm{xor}\ (4\times 2)\ \mathrm{xor}\ (5\times 6)=24$��

**��������**

�����������ṩ���������������ֱ������Ϊ������д��ĳ���

```cpp
#include<bits/stdc++.h>
using namespace std;
typedef long long ll;
namespace Generator{
typedef unsigned long long ull;
typedef __uint128_t L;
ull seed;
int p,q;
struct FastMod {
    ull b, m;
    FastMod(ull b) : b(b), m(ull((L(1) << 64) / b)) {}
    ull reduce(ull a) {
        ull q = (ull)((L(m) * a) >> 64);
        ull r = a - q * b; // can be proven that 0 <= r < 2*b
        return r >= b ? r - b : r;
    }
}F(2);
void init(){
	cin>>p>>q>>seed;//���� p,q,seed 
	assert(p!=q);
	F=FastMod(q-p+1);
}
unsigned long long rd () {
	seed ^= (seed << 13);
	seed ^= (seed >> 7);
	seed ^= (seed << 17);
	return seed;
}
void getlr(int &l1,int &r1,int &l2,int &r2){
	//�� l1,r1,l2,r2 ��Ϊ�������룬���ɵõ�һ��ѯ�� 
	l1=F.reduce(rd())+p;
	r1=F.reduce(rd())+p;
	l2=F.reduce(rd())+p;
	r2=F.reduce(rd())+p;
	if(l1>r1)swap(l1,r1);
	if(l2>r2)swap(l2,r2);
}

}
int n,m,a[100005];
int main(){
	scanf("%d%d",&n,&m);
	for(int i=1;i<=n;i++)scanf("%d",&a[i]);
	Generator::init();
	long long xorsum=0;
	for(int i=1,l1,r1,l2,r2;i<=m;i++){
		Generator::getlr(l1,r1,l2,r2);
		long long ans=/*ans������Ĵ�*/;
		xorsum^=ans*i;
	}
	cout<<xorsum;
}
```

**���ݷ�Χ**

�������ĸ�������������һʱ������ $0.5$ �룬����������ʱ������ $5$ �롣

�������ݾ����㣺$1\le n\le 10^5$��$1\le m\le 2\times 10^7$��$1\le a_i\le 4000$��$1\le p\lt q\le 4000$��$0\le seed\lt 2^{64}$��

- ������ $1$��$5$ �֣���$n,m,a_i,q\le 10$��
- ������ $2$��$20$ �֣���$n\le 10^4$��
- ������ $3$��$20$ �֣���$a_i,q\le 10$��
- ������ $4$��$55$ �֣������������ơ�

