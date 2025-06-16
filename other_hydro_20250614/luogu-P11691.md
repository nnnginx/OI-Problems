## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/ivkgc3xh.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/g6x68pxy.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/77aede4h.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/5q0pv4jf.png)

## ��Ŀ����
���ز����� #include <data.h>

�ύʱ���������ģ�壬���� include data.h�����巽������ֱ�Ӱ����ģ������Լ��������档

����˵����Ϊ�Ա��ز��Ե�˵�����ύʱ��ע�������˵����

```cpp
class Data{
	friend int main();
  private:
	unsigned short x1,x2,x3,x4;
  public:
	void add(const Data &a,const Data &b);
	void sub(const Data &a,const Data &b);
	void clr();
};
void solve(
	int n,
	int xy[][2],
	Data d[],
	int m,
	int abc[][3],
	int q,
	int lr[][2],
	Data ans[]);
```

����һ�������⣬����Ҫ���� `Data` ��ʵ�� `solve()` �����������ʹ�� `Data` ��ĳ�Ա���� `add()`��`sub()`��`clr()`���Լ� C++ �������Զ��ϳɵĺ������������캯���͸�ֵ���������

������ `Data` ���͵�Ԫ����ɵļ���Ϊ $D$��

������ $a,b,c\in D$�����������ʣ�

  - $a+b, a-b \in D$
  - $(a+b)+c=a+(b+c)$
  - $a+b=b+a$

���ڵ�λԪ $e \in D$��ʹ�ö����� $a,b\in D$�����������ʣ�

  - $a+e=e+a=a$
  - $a+(e-a)=(e-a)+a=e$
  - $a-b=a+(e-b)$

��������Ҳ���Ա���Ϊ��$(D,+,-,e)$ ����һ������Ⱥ��

���� $n$ ���㣬�� $i$ ���������� $(x_i,y_i)$ �� `Data` ���Ȩֵ $d_i$��$i=1,2,\dots,n$��

���� $m$ ����ƽ�� $(A_i,B_i,C_i)$��$i=1,2,\dots,m$��

���� $q$ ��ѯ�� $l_i,r_i$��$i=1,2,\dots,q$��

�� $i$ ��ѯ���У�����Ҫ�ش�һ�������еİ�ƽ��Ľ��ĵ�Ȩ�ͣ�������˵��

�輯�� $S_i = \{ k \mid \forall l_i \le j \le r_i, A_jx_k + B_jy_k \ge C_j \}$���� $\sum\limits_{k \in S_i} d_k$��

## ��ʾ
Idea��nzhtl1477��Solution��nzhtl1477&ccz181078��Code��ccz181078��Data��ccz181078

### �ӿ�˵��

ʹ�� `a.clr()` �������Խ� $a$ ��Ϊ��λԪ $e$��

ʹ�� `a.add(b,c)` �������Խ� $a$ ��Ϊ $b+c$��

ʹ�� `a.sub(b,c)` �������Խ� $a$ ��Ϊ $b-c$��

ʹ�� `a=b` ���Խ� $a$ ��Ϊ $b$��

### ����˵��

����Ҫʵ�ֵĺ��� `solve` �Ľӿ���Ϣ���£�

```cpp
void solve(
	int n,
	int xy[][2],
	Data d[],
	int m,
	int abc[][3],
	int q,
	int lr[][2],
	Data ans[]);
```

����ʱ���������ǡ�õ��� `solve` һ�Ρ�

�� `solve` �����Ĳ����У�$x_i$ ��Ӧ `xy[i][0]`��$y_i$ ��Ӧ `xy[i][1]`��$d_i$ ��Ӧ `d[i]`��

$A_i,B_i,C_i$ ��Ӧ `abc[i][0],abc[i][1],abc[i][2]`��

$l_i,r_i$ ��Ӧ `lr[i][0],lr[i][1]`���� $i$ ��ѯ�ʵĴ���Ҫ�������� `ans[i]`��

$n,m,q$ ��Ӧ `n,m,q`��

����Խ�������ζ�Ԫ�صĸ�ֵ���������� `clr()` �����ĵ��ã������� `add()` �� `sub()` �Ĵ���֮�Ͳ��ܳ��� $4\times 10^7$��

�� `C++` ����ѡ�֣���ȷ����ĳ���ͷ��

```cpp
#include "data.h"
```

����Ŀ¼�µ� `grader.cpp` �������ṩ�Ľ�����ο�ʵ�֣����ղ���ʱ���õĽ�����ʵ����òο�ʵ��������ͬ�����ѡ�ֵĽⷨ��Ӧ������������ʵ�֡�

�� `C++` ���Ե�ѡ�֣�

����Ҫ�������ύ��������Ϊ `chesed.cpp`�����ڱ���Ŀ¼��ʹ�������������õ���ִ�г���

```
g++ grader.cpp chesed.cpp -o chesed -O2 -lm
```

���ڱ���õ��Ŀ�ִ�г���

�ȴӸò��Ե�����������ж������ݡ�

�������֮�󣬽����⽫����ǡ��һ�κ��� `solve`�����������ݲ�����ĺ�����

��ĺ�����ȷ���غ󣬽����������㷵�صĽ��������ļ������ÿ��ѯ�ʵĴ𰸣����������Ĵ𰸺Ͷ�Ӧ���Ե������ļ�����ĩ�ո�����ȫһ�£����ж���ͨ���ò������ݡ�

### ������Լ��

���� $25\%$ �����ݣ����� $n,m,q\le 100$��

�������� $25\%$ �����ݣ����� $q\le 100$��

�������� $25\%$ �����ݣ����� $l_i=r_i$��$x_i,y_i$ �����������ݷ�Χ�ھ������ѡȡ��

�� $100\%$ �����ݣ����� $1\le n\le 2\times 10^5$��$1\le m\le 10^4$��$1\le q\le 10^5$��$|A_j|,|B_j|\le 10^4$��$|x_i|,|y_i|,|C_j|\le 10^5$��$B_j>0$��$C_j<0$��$-10^6\le C_j<0$��$1\le l_i\le r_i\le m$��



