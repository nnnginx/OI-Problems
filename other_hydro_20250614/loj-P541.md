## ��Ŀ����

**���� C/C++ ʱ�� 2.5 �룬Pascal ʱ�� 5 �롣��󽫸�ʱ���ز����� Pascal �ύ��**

��֪�������û����������ϵ�е�һ�׸裬�������ÿ����������ϰ��˻��Ĺ��¡�  
   
��һ�Σ�����˾�������򱻰��С���ħ��֮����������ϲ���Ⱥ�裬һ����Ҫ�������򿪿��������˺�������
  
�����ʵ�Ǳ�ú��˵ģ�ÿ����趼��һ���Ǹ���������ţ��� $0$ ��ʼһֱ�����������������������ħ��ɳ������һ���˺�衣  

һ��ʼ�������Ѿ����˱��Ϊ $0$ �� $a$ �ĺ�裨ע�� $a=-1$ �ͱ�ʾ��ʼ������û���κκ�裩��Ȼ�����������ħ�ݵ�·���� $m$ ��ʱ�̣�ÿ��ʱ�̶��ᷢ��һ���¼���

> * ��һ���¼�����������һ�����꣬����һ�����Ϊ $x$ �ĺ�裨�����ϳ�ʼû�����ֱ�ŵĺ�裬֮ǰҲ���������ͬ��ŵĺ�裩��  
> * �ڶ����¼���һ��Ŀǰ�ڿ����ϵı��Ϊ $x$ �ĺ��ɳ��˿�����  
> * �������¼���ħ��ɳ��Ŀǰ���ڿ����ϵ�����ɳ�ȥ�ĺ�����˿����ϣ����һ����������ɳ�ȥ���������Ȼ���ٷɳ�ȥ��������Ϊ��ɳ�ȥ��ʱ��Ϊ���һ�ηɳ�ȥ��ʱ�䣩��  


����������Щ�¼�ʵ����̫�鷳�ˣ�������ħ��ɳ����һ������Ϊ $m$ ���������� $p$ ������ÿ��ʱ�̷������¼���

> * ������� $p$ ������Ԫ�ؾ�Ϊ $[-1,b)$ ��������  
> * �� $p_i=-1$ ���ʾʱ�� $i$ �����˵������¼��������ʱ�����������������ķɳ�ȥ�ĺ�裬�����ħ��ɳ����ûת���������Ӵ˴��¼���  
> * ���������ʱ�� $i$ ���Ϊ $p_i$ �ĺ���ʼ���ڿ�����Ҳ����û��ͨ����һ���¼���������ʾʱ�� $i$ ������һ������Ϊ $p_i$ �ĺ��ĵ�һ���¼���
> * ���������ʱ�� $i$ ���Ϊ $p_i$ �ĺ���ڿ����ϣ����ʾʱ�� $i$ ������һ�����Ϊ $p_i$ �ĺ��ɳ������ĵڶ����¼���
> * ���򣬱�ʾʱ�� $i$ �����˵������¼��������ʱ�����������������ķɳ�ȥ�ĺ�裬����Ӵ˴��¼���  

���ĳ��ʱ�̵��¼������ӣ���ô����**��ִ�ж�Ӧ�Ĳ�����Ҳ�������ʱ�Ĵ�**��  

��������һ���ڷܵ��ˣ�ÿ��ʱ�̹���������ʱ�� $i$ �������¼������һ��ʱ�̷������¼��������ˣ��Ͳ���Ϊ���ʱ�̷������¼������� $ans_i$ ��ʾʱ�� $i$ ���󿨳������б��С�� $ans_i$ �ĺ�趼�����ˣ������Ϊ $ans_i$ �ĺ��û�г��֣�����Ȼ���ֵ��Ψһ�ģ�����Ȼ���ʱ�� $i$ û�з����¼������� $ans_i=0$ ��  

������� $1 \leq i \leq m$ ����� $ans_i\times (i^2+7i)\ mod\ 998244353$ �����͡�  

## �����ʽ

��һ��һ������ $T$ ����ʾ����������  

�������� $T$ �У�ÿ�б�ʾһ�����ݡ�  

ÿ������������ $m,\mathrm{seed},a,b,c,d$ �������������� $m,a,b$ ����������������ͬ��  
$d$ ��ʾ�Ƿ�ֻ���ǵ�һ���¼���$d$ ��ȡֵΪ $0$ �� $1$ ��Ϊ����������� $d=1$ ʱ����������еĵڶ����¼���������¼������ӵĺ����������������  
$\mathrm{seed},c$ ��������������Ĳ�����

����ʹ������ʵ�ֵ������������ $\mathrm{randnum}()$��ÿ������������������� $\mathrm{seed}$ �ĳ�ʼֵ��

```
unsigned 32bit integer seed

function randnum()
	seed = seed xor (seed lsh 13)
	seed = seed xor (seed rsh 17)
	seed = seed xor (seed lsh 5)
	return seed
end function
```

���� $p[]$ �Ĵ������£�

```
for i = 1 to m by step 1
	if randnum() mod c == 0 then
		p[i] = -1
	else
		p[i] = randnum() mod b
	end if
end for
```

�����ڡ����ݷ�Χ����ʾ��������ṩ��������һ���������ģ�壨Ҳ�����ڸ����ļ������أ�������㲻��Ҫ�����������


## �����ʽ

ÿ���������һ�б�ʾ�𰸡�

```input1
1
7 327711436 4 6 3 0
```

```output1
292
```

## ���ݷ�Χ����ʾ

**���� C/C++ ʱ�� 2.5 �룬Pascal ʱ�� 5 �롣��󽫸�ʱ���ز����� Pascal �ύ��**

�����������ݣ�$1 \leq m \leq 10^6$��$1 \leq T \leq 50$ �� $-1 \leq a \leq m$ ��  $1 \leq b \leq 2\times m$ �� $1 \leq c \leq 10^7$ �� $0 \leq d \leq 1$ ��

$d$ ��ʾ�Ƿ�ֻ���ǵ�һ���¼���$d$ ��ȡֵΪ $0$ �� $1$ ��Ϊ����������� $d=1$ ʱ����������еĵڶ����¼���������¼������ӵĺ����������������  
ע�⣬$d=1$ ʱԭ���Ϸ����¼�ҲҪ�����ӣ��ʼ�ʹ��û���õ�������ʣ�ҲҪ�ǵ��ж� $d=1$ ������������Ե� $7$ ����Ĳ��Ե�Ҳ�п��ܳ��� $d=1$ �����ݡ�

|���Ե� #|$m$ ������|$T$������|��������|
|:-:|:-:|:-:|:-:|
|$1$|$m \leq 3000$|$T \leq 20$|-|
|$2$|$m \leq 3000$|$T \leq 25$|-|
|$3$|$m \leq 3000$|$T \leq 30$|-|
|$4$|$m \leq 10^5$|$T \leq 20$|-|
|$5$|$m \leq 10^5$|$T \leq 30$|-|
|$6$|$m \leq 10^5$|$T \leq 50$|-|
|$7$|$m \leq 10^6$|$T \leq 50$|$d=1$|
|$8$|$m \leq 8\times 10^5$|$T \leq 50$|-|
|$9$|$m \leq 10^6$|$T \leq 50$|-|
|$10$|$m \leq 10^6$|$T \leq 50$|-|

#### �������ģ��
**�������ģ����������ʱ��ֱ�Ϊ��C/C++Լ 400 ms��Pascal Լ 2000 ms**

```c++
//C++
#include<cstdio>

namespace IO{
	int c;
	unsigned int seed;
	unsigned int randnum(){
		seed^=seed<<13;
		seed^=seed>>17;
		seed^=seed<<5;
		return seed;
	}

	inline int read(int &x){scanf("%d",&x);return x;}
	inline void init_case(int &m,int &a,int &b,int &d,int p[]){
		scanf("%d%u%d%d%d%d",&m,&seed,&a,&b,&c,&d);
		for(int i=1;i<=m;i++){
			if(randnum()%c==0)p[i]=-1;
			else p[i]=randnum()%b;
		}
	}

	inline void update_ans(unsigned int &ans_sum,unsigned int cur_ans,int no){
		const static unsigned int mod=998244353;
		ans_sum^=(long long)no*(no+7)%mod*cur_ans%mod;
	}
}
using IO::read;
using IO::init_case;
using IO::update_ans;
/*
һ��ʼ�����read(T)������������T
������ÿ�����ݿ�ʼʱ�����init_case(m,a,b,d,p)����m,a,b,d,p[]
ÿ�����ݿ�ʼʱ����һ����ʼ��Ϊ0��32λ�޷������α���ans_sum�洢�𰸣�Ȼ�����ÿ��i��
��32λ�޷������α���cur_ans�洢��i�δ𰸣�������update_ans(ans_sum,cur_ans,i)���¡�������ans_sum���ɡ�
*/

//ʾ�����룺
/*
int main(){
	static int p[2000005];
	int T;read(T);
	int m,a,b,d;
	while(T--){
		unsigned int ans_sum=0,cur_ans=0;
		init_case(m,a,b,d,p);
		for(int i=1;i<=m;i++){
			......//�������
			update_ans(ans_sum,cur_ans,i);
		}
		printf("%u\n",ans_sum);
	}
	return 0;
}
*/
```
```c
//C
#include<stdio.h>

int _IO_c;
unsigned int seed;
unsigned int randnum(){
	seed^=seed<<13;
	seed^=seed>>17;
	seed^=seed<<5;
	return seed;
}

inline int read(int *x){scanf("%d",x);return *x;}
inline void init_case(int *m,int *a,int *b,int *d,int p[]){
	int i;
	scanf("%d%u%d%d%d%d",m,&seed,a,b,&_IO_c,d);
	for(i=1;i<=*m;i++){
		if(randnum()%_IO_c==0)p[i]=-1;
		else p[i]=randnum()%*b;
	}
}

inline void update_ans(unsigned int *ans_sum,unsigned int cur_ans,int no){
	const static unsigned int mod=998244353;
	*ans_sum^=(long long)no*(no+7)%mod*cur_ans%mod;
}

/*
һ��ʼ�����read(&T)������������T
������ÿ�����ݿ�ʼʱ�����init_case(&m,&a,&b,&d,p)����m,a,b,d,p[]
ÿ�����ݿ�ʼʱ����һ����ʼ��Ϊ0��32λ�޷������α���ans_sum�洢�𰸣�Ȼ�����ÿ��i��
��32λ�޷������α���cur_ans�洢��i�δ𰸣�������update_ans(&ans_sum,cur_ans,i)���¡�������ans_sum���ɡ�
*/

//ʾ�����룺
/*
int main(){
	static int p[2000005];
	int T;int m,a,b,d,i;
	read(&T);
	while(T--){
		unsigned int ans_sum=0,cur_ans=0;
		init_case(&m,&a,&b,&d,p);
		for(i=1;i<=m;i++){
			......//�������
			update_ans(&ans_sum,cur_ans,i);
		}
		printf("%u\n",ans_sum);
	}
	return 0;
}
*/
```
```pascal
//Pascal

type
	pointer_32=^longint;
var
	_IO_c:longint;
	seed:Cardinal;
	p:array[0..2000004]of longint;
	T,m,a,b,d,i:longint;
	ans_sum,cur_ans:Cardinal;

function randnum():Cardinal;
begin
	seed:=seed xor (seed shl 13);
	seed:=seed xor (seed shr 17);
	seed:=seed xor (seed shl 5);
	exit(seed);
end;

procedure init_case(var m,a,b,d:longint;p:pointer_32);inline;
var
	i:longint;
begin
	read(m,seed,a,b,_IO_c,d);
	for i:=1 to m do begin
		if randnum() mod _IO_c=0 then p[i]:=-1
		else p[i]:=randnum() mod b;
	end;
end;

procedure update_ans(var ans_sum:Cardinal;cur_ans:Cardinal;no:longint);inline;
const
	mod_val:Cardinal=998244353;
	calc:int64=1;
begin
	ans_sum:=ans_sum xor (calc*no*(no+7) mod mod_val*cur_ans mod mod_val);
end;

{
һ��ʼ�����read(T)������������T
������ÿ�����ݿ�ʼʱ�����init_case(m,a,b,d,p)����m,a,b,d,p[]
ÿ�����ݿ�ʼʱ����һ����ʼ��Ϊ0��32λ�޷������α���ans_sum�洢�𰸣�Ȼ�����ÿ��i��
��32λ�޷������α���cur_ans�洢��i�δ𰸣�������update_ans(ans_sum,cur_ans,i)���¡�������ans_sum���ɡ�
}

//ʾ�����룺
{
begin
	read(T);
	while T>0 do begin
		dec(T);
		ans_sum:=0;cur_ans:=0;
		init_case(m,a,b,d,p);
		for i:=1 to m do begin
			......//�������
			update_ans(ans_sum,cur_ans,i);
		end;
		writeln(ans_sum);
	end;
end.
}
```

