## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/gu2canu2.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/zr2prltd.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/450q6z6z.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/10ntmhxz.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/gtn14jr6.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/4o7rowbj.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/3rj866um.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/13cscyn0.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/lsf5mhce.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/1l09guml.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/ej6qg7v0.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/hjkcg54p.png)

## ��Ŀ����
�������۰�Ⱥ $(D,+,e)$������ $D$ �е�Ԫ�ع��ɵ����� $a_1,\dots,a_n$����ֵ��Ϊ $e$��֧�� $m$ �β�����ÿ�β��������ǵ����޸ģ��������͡�

����ÿ���޸Ĳ���ʹ�� $+$ �Ĵ��������� $M_1$��

����ÿ�β�ѯ����ʹ�� $+$ �Ĵ��������� $M_2$��

�۰�Ⱥ�Ļ������ʣ�

$\forall a\in D,\; e+a=a+e=a$

$\forall a,b,c\in D,\;(a+b)+c=a+(b+c)$



����һ�������⣬����Ҫ����ͷ�ļ� `lib.h`���������ݷ��ڳ������ǰ�档

�·���ͷ�ļ� `lib.h` ���������£�

```c++
struct Data{
	unsigned short a,b,c,d;
};
Data operator+(Data a,Data b);

void init(int n,int k,Data d);
void update(int x,Data d);
Data query(int l,int r);
```

���� `Data` ��ʾ $D$��`Data operator+` ��ʾ $+$��������������ⲿ�ֵ�ʵ�֣�

����Ҫʵ�֣�

`init` ���ڳ�ʼ����`n,k,d` ���α�ʾ $n,M_2$ �� $D$ �ĵ�λԪ $e$�������ʹ�� $+$�������� $e+e=e$ �����ܵó����õĽ����

`update` ��ʾһ���޸Ĳ������� $a_x$ �޸�Ϊ $d$��

`query` ��ʾһ�β�ѯ����͵Ĳ�������ѯ $a_l+a_{l+1}+\dots+a_r$����ѯ���Ӧ����Ϊ����ֵ���أ�

## ��ʾ
Idea��ccz181078��Solution��ccz181078��Code��ccz181078��Data��ccz181078

���������ݣ����� $n=10^5,\;m=2\times 10^5$

| ���ݵ��� | $M_1$ | $M_2$ | ���� |
| ---------- | ----- | ----- | ---- |
| 1          | 4000  | 2     | 11   |
| 2          | 700   | 3     | 7    |
| 3          | 400   | 4     | 5    |
| 4          | 200   | 5     | 4    |
| 5          | 200   | 6     | 4    |
| 6          | 100   | 7     | 3    |
| 7          | 80    | 8     | 3    |
| 8          | 60    | 9     | 3    |
| 9          | 2811  | 2     | 16   |
| 10         | 542   | 3     | 11   |
| 11         | 272   | 4     | 8    |
| 12         | 137   | 5     | 7    |
| 13         | 113   | 6     | 5    |
| 14         | 75    | 7     | 5    |
| 15         | 69    | 8     | 4    |
| 16         | 48    | 9     | 4    |

`lib\down` Ŀ¼Ϊ�·��Ľ������ļ�

`lib\require` Ŀ¼Ϊ�����õĽ������ļ�

`data` Ŀ¼Ϊ�����õĲ��Ե�

`data2` Ŀ¼Ϊ�·�������

