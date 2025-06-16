## ��Ŀ����
������ײ�����Ƴ� FAOI Round 6.

> Draw me to the light, let the curse be lifted  
We can rise above the roar  
With the bite of every devil  
We've felled before  
Drown them out  
Let the fog give way to clarity  
There is power in the strain of every drop I bleed  
I am the venom and the cure  
Take me  
Through the fear, through the heart that's broken  
Our world lies in wait for me  
Every tear, every scar left open  
This is the taming of the beast  
I'll end this war you started  
I'll stitch this wound with bloodshed  
You are my wicked victory  

<https://music.163.com/#/song?id=2672191019>

[](Ϊ���ý�������������������_`Ready`_����������_`fseek`_����ƶ�����ָ�뵽��ͷ��������һ�д��ո���ַ�����Ȼ���ٿ�ʼ������⡣���벻Ҫ������ʾ��һ�㡣�������������࣬������һ��Ҫ��ô������ǳ���Ҫ������)

## ��Ŀ����
����һ������**��ͨ**ͼ���ߴ�Ȩ�����ܴ����ر��Ի����� $q$ �β�ѯ��ÿ�θ��� $x,y,z$���������� $x$ Ϊ��㣬$y$ Ϊ�յ��·������Ҫ��Ϊ��·�����У���Ȩ�� $\bmod\ z$ ����Сֵ�Ƕ��١�

### ������ʽ

[](Ϊ���ý�������������������_`Ready`_����������_`fseek`_����ƶ�����ָ�뵽��ͷ��������һ�д��ո���ַ�����Ȼ���ٿ�ʼ������⡣���벻Ҫ������ʾ��һ�㡣�������������࣬������һ��Ҫ��ô������ǳ���Ҫ������)**����Ϊ�����⣬ֻ֧�� C++ �����ύ�����Ҳ�֧�� C++14 (GCC 9)��**

����Ҫ��д��������������

```cpp
void Ready(int T, int subtask_id)
```

�ú�����ÿ�����Ե��н������һ�Σ�����������ʾ�ò��Ե�������������������š���������������Ϊ $-1$��

```cpp
void Set(int n, int m, int q, vector <int> u, vector <int> v, vector <int> w)
```

�ڵ��� `Ready` ֮�󣬸ú����ᣨ��ÿ�����Ե��У������� $T$ �Σ����� $n,m$ �ֱ��ʾͼ�ı����͵�����$u,v,w$ �Ĵ�С��Ϊ $m$��$u[i],v[i],w[i]$ ��ʾͼ��һ���ߡ�

```cpp
int Go(int x, int y, int z)
```

ÿ�ε��� `Set` ֮�󣬸ú����ᣨ��ÿ�������У������� $q$ �Σ�ÿ�ε��ñ�ʾһ�β�ѯ������ֵӦΪ���β�ѯ�Ĵ𰸡�

�����ֱ�����·��ļ��е� `template.cpp` Ϊ������д��

## �����ʽ
**���¸�ʽֻ�Ա��ز�����Ч�����������ĺ�����ʵ��������ͬ����ʵ�������У��벻Ҫ��ͼ�ӱ�׼���루stdin����ȡ�κ����ݡ�**

**�����ж������ݡ�**

��һ�������Ǹ����� $T$ �� $\text{subtask\_id}$���ֱ��ʾ���������� Subtask ��š�

�ر�أ��������� $\text{subtask\_id}=-1$��

����ÿ�����ݣ�
- ��һ���ǿ��С�
- �ڶ��������Ǹ����� $n,m,q$��
- ������ $m$ �У�ÿ�������Ǹ����� $u,v,w$����ʾһ���ߡ�
- ������ $q$ �У�ÿ������������ $x,y,z$����ʾһ�β�ѯ��

## �����ʽ
**���¸�ʽֻ�Ա��ز�����Ч�����������ĺ�����ʵ��������ͬ����ʵ�������У��벻Ҫ��ͼ���׼�����stdout����ӡ�κ����ݡ�**

����ÿ�����ݣ�
- ��һ���ǿ��С�
- ���� $q$ �У�ÿ��һ���Ǹ���������ʾ�𰸡�

```input1
2 -1

2 1 1
1 2 1
1 2 2

3 3 1
1 2 1
2 3 1
1 3 1
1 3 2

```

```output1

1

0

```

## ��ʾ
#### ���������͡�

���ڵ� $1$ �����ݵ�Ψһһ��ѯ�ʣ�����·�������� $1\to 2\to 1\to \dots \to 1\to 2$������֤������·����Ȩֵ��Ϊ $1$��

���ڵ� $2$ �����ݵ�Ψһһ��ѯ�ʣ�·�� $1\to 2\to 3$ ȨֵΪ $2\bmod 2=0$��·�� $1\to 3$ �Ĵ�Ϊ $1\bmod 2=1$�����Դ�Ϊ $0$��

#### �����ݷ�Χ��

���� $100\%$ �����ݣ�$0\le T\le 1.5 \times 10^4$��$-1 \le \text{subtask\_id} \le 9$��$0\le n,m,q\le 10^6$��$1\le u,v,x,y\le n$��$0\le w\le 10^9$��$1\le z\le 10^9$����֤ͼ��ͨ��

�����ظ����е� `judge_result.jpeg` ���˽⽻������ռ����Դ�Ĺ�ģ������㲻�����ظ����Ļ���������������һ�仰����һ�£���֤�����������ʱ�䲻���� 0.15 �룬ռ�õ��ڴ治���� 60 MB��

**���⿪��������������ԡ�**

- Subtask 0 - Subtask 4��10 pts����$n,m,q,w,z\le 10$��$T \le 1.5 \times 10^4$��
  - Subtask 0��2 pts����$n=0$��
  - Subtask 1��2 pts����$n=1$��
  - Subtask 2��1 pts����$n=2$��$m \le 3$��
  - Subtask 3��4 pts����$n \le 4$��$m \le 6$��$w \le 8$��
  - Subtask 4��1 pts������ Subtask 0 - Subtask 4 �����������ơ�
- Subtask 5 - Subtask 9��90 pts����$n,m,q\le 10^6$��$w,z \le 10^9$��$T=1$��
  - Subtask 5��20 pts����$n,m,q,w,z\le 100$��
  - Subtask 6��20 pts����$n,m,q,w,z\le 10^3$��
  - Subtask 7��10 pts����$w,z\le 5$��
  - Subtask 8��10 pts����$w=1$��
  - Subtask 9��30 pts������ Subtask 5 - Subtask 9 �����������ơ�


Idea��ppip��Solution������ţ�̣�Code��ppip��Data��035966_L3

[��ε��ԣ�](https://www.luogu.com.cn/paste/3x0kjgps)

