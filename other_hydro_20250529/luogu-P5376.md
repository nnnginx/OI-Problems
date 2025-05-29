## ��Ŀ����
> �������ǻ���һ�¾���������������⣺
>
> ������ $A$ ����һ�������䣬��Ҫ�ߵ�Ŀ�� $B$ �㡣�����ߵĹ��򣺿������ϡ��������ҡ�ͬʱ�������� $C$ ����һ���Է������������ڵĵ��������Ծһ���ɴ�ĵ��Ϊ�Է���Ŀ��Ƶ㣬��˳�֮Ϊ�����������䡹��
>
> �����������ʾ��$A$ �� $(1,1)$ ��$B$ �� $(N,M)$ ��ͬ�����λ����������Ҫ�����ġ�
>
> ����Ҫ����������� $A$ ���ܹ����� $B$ ���·�����������������λ���ǹ̶������ģ�����������һ������һ����
>
> **��ע�⣬�������������뱾���޹أ�**

Kiana ϲ�������壬������ϲ������������������Ϸ���ڴ�ͳ�Ĺ����������У�Kiana ��Ҫ����һ���������ߵ��յ㣬��·�бܿ�һ���Է�����Ĺ�����Ȼ���װ�����㲢ѯ�������㵽�յ��·��������

�ڽ���Ĺ��������Ϸ�У�Kiana ���ǿ���һ������һ�� $N\times M$ ���������ƶ�����ʼʱ��λ�����·�����Ϊ $(1,1)$ λ�ã���Ϊ�������Ѷȣ�Kiana ����Ϸ����������һЩ�޸ġ���ͳ�Ĺ�����ÿ��ֻ�����ϻ������ƶ� $1$ ��Kiana �涨�Լ��Ĺ��������������һ���������Ϸ��ƶ� $1$ �񣬼������ǰ��λ������ $(x,y)$ ��������һ�������ߵ� $(x+1,y)$ ��$(x,y+1)$ �� $(x+1,y+1)$ �е�����һ������ȥ��ͬʱ Kiana ��Ϊ����������ƶ�������ĳһ��ʱ���ƶ��ķ����ҡ��ϻ����ϣ���ͬ�������ַ������ǲ�ͬ�ģ������ $(1,1)$ ���ߵ� $(1,2)$ ���ߵ� $(2,2)$ ���� $(1,1)$ ���ߵ� $(2,1)$ ���ߵ� $(2,2)$ �ʹ� $(1,1)$ ֱ���ߵ� $(2,2)$ �����ֲ�ͬ���ƶ�������

��Σ�����������յ㲻����һ���ض���λ�ã�Kiana �涨����Դ����̵��Ϸ����ҷ��߳����̣���ʱ����Ϊ��Ϸ�ɹ���ע�����߳�����ʱ��Ȼ�з���ѡ��Ĳ�ͬ��������������λ�� $(1,M)$ ��������һ�����������һ��������������ַ�ʽ�߳����̣���������λ�� $(N,M)$ ��������һ�����������ϡ����һ��������������ַ�ʽ�߳����̣��Բ�ͬ�ķ�ʽ�߳�������Ȼ�������ǲ�ͬ���ƶ�������

���⣬�Է���Ĺ�����Χ�������й��ɵļ���λ�ã����� Kiana �涨�õ� $K$ ���ض����꣬��Ҫ����������ƶ��Ĺ����в����ߵ��� $K$ ��������κ�һ���ϣ��ڳ���Щ���������λ���Ϲ����䶼���԰����������ƶ���

���� Kiana ��֪������������ж����ֲ�ͬ���ƶ����������߳����̣�����𰸿��ܷǳ�����ֻ��֪���������� $59393$ ȡģ��Ľ���������������㣬����ϣ����������������



## �����ʽ
��һ�а����������� $N$ ��$M$ �� $K$ ���ֱ��ʾ���̵����귶Χ��Է���Ĺ������������� Kiana �涨�Ĳ��ܾ���������������

������ $K$ �У��� $i$ �а������������� $X_i$ �� $Y_i$ ����ʾ�Է���ĵ� $i$ ����������Ϊ $(X_i,Y_i)$ ��

�����������ݣ���֤ $1\leq N\leq 10^9,1\leq M\leq 10^5,0\leq K\leq 20,1\leq X_i\leq N,1\leq Y_i\leq M$��$(1,1)$ һ�����ᱻ�Է��������ұ������ĸ����в���������������ͬ�ĸ��ӡ�

## �����ʽ
���һ��һ����������ʾ�������߳����̵ķ������� $59393$ ȡģ��Ľ����



```input1
3 3 1
2 2
```

```output1
24
```

## ��ʾ
### ��������

�� $\uparrow$ ��ʾ�����������ƶ���һ���� $\rightarrow$ ��ʾ�����������ƶ���һ���� $\nearrow$ ��ʾ�������������ƶ���һ���ɴ˿��Լ��������͵ı�����

$24$ ���ƶ��������£�

$(\uparrow\uparrow\uparrow)$��$(\uparrow\uparrow\nearrow)$��$(\uparrow\uparrow\rightarrow\uparrow)$��$(\uparrow\uparrow\rightarrow\nearrow)$��

$(\uparrow\uparrow\rightarrow\rightarrow\uparrow)$��$(\uparrow\uparrow\rightarrow\rightarrow\nearrow)$��$(\uparrow\uparrow\rightarrow\rightarrow\rightarrow)$��$(\uparrow\nearrow\uparrow)$��

$(\uparrow\nearrow\nearrow)$��$(\uparrow\nearrow\rightarrow\uparrow)$��$(\uparrow\nearrow\rightarrow\nearrow)$��$(\uparrow\nearrow\rightarrow\rightarrow)$��

$(\rightarrow\rightarrow\rightarrow)$��$(\rightarrow\rightarrow\nearrow)$��$(\rightarrow\rightarrow\uparrow\rightarrow)$��$(\rightarrow\rightarrow\uparrow\nearrow)$��

$(\rightarrow\rightarrow\uparrow\uparrow\rightarrow)$��$(\rightarrow\rightarrow\uparrow\uparrow\nearrow)$��$(\rightarrow\rightarrow\uparrow\uparrow\uparrow)$��$(\rightarrow\nearrow\rightarrow)$��

$(\rightarrow\nearrow\nearrow)$��$(\rightarrow\nearrow\uparrow\rightarrow)$��$(\rightarrow\nearrow\uparrow\nearrow)$��$(\rightarrow\nearrow\uparrow\uparrow)$��

### ��Ȩ��Ϣ

���� THUPC��THU Programming Contest���廪��ѧ������ƾ�����2019��

������Դ���� <https://github.com/wangyurzee7/THUPC2019> �鿴��

