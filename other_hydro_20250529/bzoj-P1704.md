## ��Ŀ����
ũ��Լ���� $n$ ֻţվ��һ�ţ���һЩ�ܹԵ�ţ��ǰվ�š�������Щ���Ե�ţȴ����վ�š�ũ��Լ����Ҫ�����е�ţ����ǰվ�š����˵���Լ���������һ���Զ�ת������������Ļ�����ʹ $k$ ֻ������ţת����ΪԼ�����������ı� $k$ �ļ�ֵ������������ $k$��ʹ��ת���� $m$ �ﵽ��С��ͬʱҪ�����Ӧ�� $m$��
## �����ʽ
 ��һ�У����� $n$��  
 �ڶ��е��� $n+1$ �У��� $i+1$ �б�ʾţ $i$ �ĳ���`F` ��ʾ��ǰ��`B` ��ʾ����
## �����ʽ
 һ�����������ֱ��� $k$ �� $m$���м��ÿո������

```input1
7
B
B
F
B
F
B
B
```
```output1
3 3
```
## ����˵��

INPUT DETAILS:  
There are seven cows and they are facing backward, backward, forward, backward, forward, backward, and backward, respectively.

OUTPUT DETAILS:  
For $k = 3$, the machine must be operated three times: turn cows $(1,2,3)$,$(3,4,5)$, and finally $(5,6,7)$:
```
 B > F   F   F
 
 B > F   F   F
 
 F > B > F   F
 
 B   B > F   F
 
 F   F > B > F
 
 B   B   B > F
 
 B   B   B > F
```
## ��ʾ
�� $k=3$ ʱ����Ļ�����ת $3$ �Σ�$(1,2,3),(3,4,5)$ �� $(5,6,7)$��
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1\le k\le n\le 5\times 10^3$��
## ��Ŀ��Դ
Gold