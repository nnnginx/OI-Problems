## ��Ŀ����
ǰ�ԣ���Ȼ SCR �Ѿ������� JROI������Ϊ JROI �ĸ����ˣ��һ�����Ҫ��лһ�� SCR �������**��˽**���ס����ڶԳ����˵ľ��⡣���ǲ�������Ŀ��������������ĸĶ���ֻ�����**С���������ν�**����䡣

--------------

�X�m�����������ȻҪ��һ����Ϸ�ˡ�

С L �Ǹ�ϲ�������ĳ�����������������ѧ���������Ļ������㣬���ڴ����ʱ���������Լ��������ĳ��̡��������Ļ���ǽ����������ۣ�������һ��������뷨��

## ��Ŀ����
С L �� $n$ ������ $\overrightarrow{a_1},\overrightarrow{a_2}\ldots\overrightarrow{a_n}$����ϣ�����ܹ������ش������������⡣

+ ���ڸ����� $l,r$����� 

$$\sum\limits_{i=l}^{r-1}\sum\limits_{j=i+1}^{r}\overrightarrow{a_i}\cdot\overrightarrow{a_j}$$


+ ���ڸ����� $l,r$����� 

$$\sum\limits_{i=l}^{r-1}\sum\limits_{j=i+1}^{r}\overrightarrow{a_i}\oplus\overrightarrow{a_j}$$

����ʱ������ƣ���Щ����Ҳ�᲻�Ϸ����仯��С L ϣ�����ڷ����仯����Ȼ�ܸ����𰸡�

## �����ʽ
��һ���������� $n,m$���ֱ�������������Ͳ���������  

������ $n$ �У�ÿ���������� $x,y$���� $i$ �б�ʾ���� $\overrightarrow{a_i}$��  

������ $m$ �У�ÿ��������һ������ $opt$ ��ʾ������ţ�֮�������ɸ�������ʾһ�β�����һ�����������ֲ�����

1. ������������ $i,x,y(1\leq i\leq n)$���� $\overrightarrow{a_i}$ ���� $(x,y)$��
1. ������������ $i,x,y(1\leq i\leq n)$���� $\overrightarrow{a_i}$ ��ȥ $(x,y)$��
1. ������������ $i,t(1\leq i\leq n)$���� $\overrightarrow{a_i}$ �޸�Ϊ $t\overrightarrow{a_i}$��
1. ������������ $l,r(1\leq l<r\leq n)$���� $\sum\limits_{i=l}^{r-1}\sum\limits_{j=i+1}^{r}\overrightarrow{a_i}\cdot\overrightarrow{a_j}$��
1. ������������ $l,r(1\leq l<r\leq n)$���� $\sum\limits_{i=l}^{r-1}\sum\limits_{j=i+1}^{r}\overrightarrow{a_i}\oplus\overrightarrow{a_j}$��

## �����ʽ
�������еĵ��ĺ͵����ֲ�����һ����һ��������Ϊ��β����Ĵ𰸡�

```input1
3 5
1 1
4 5
1 4
1 1 3 6
2 3 3 0
4 2 3
3 2 3
5 1 3
```

```output1
12
84
```

## ��ʾ
#### ���� 1 ����

ǰ���β��������������ֱ�Ϊ $(4,7),(4,5),(-2,4)$��֮��ѯ�ʽ��Ϊ $4 \times(-2)+5\times4=12$��

��һ�β��������������ֱ�Ϊ $(4,7),(12,15),(-2,4)$��ѯ�ʽ��Ϊ $(4\times15-7\times12)+[4\times4-7\times(-2)]+[12\times4-15\times(-2)]=-24+30+78=84$

-----------
#### ���ݹ�ģ��Լ��
**��������������**��
+ Subtask 1 ( $20\%$ )��$n,m\leq 100$��
+ Subtask 2 ( $30\%$ )��û�в����塣
+ Subtask 3 ( $50\%$ )��������Ҫ��

���� $100\%$ �����ݣ�$2\leq n\leq 10^5$��$1\leq m\leq 10^5$��**��֤��������ʱ�̵����� $\overrightarrow{a_i}$������ $-1000\leq x_i,y_i\leq 1000$**��

-----------
#### ������������

�������� $\overrightarrow{a},\overrightarrow{b}$ �ͳ��� $\lambda$���ٶ� $\overrightarrow{a},\overrightarrow{b}$ �������ʾ�ֱ�Ϊ $(x_a,y_a),(x_b,y_b)$��

+ $\overrightarrow{a}+\overrightarrow{b}=(x_a+x_b,y_a+y_b)$  
+ $\overrightarrow{a}-\overrightarrow{b}=(x_a-x_b,y_a-y_b)$  
+ $\lambda\overrightarrow{a}=(\lambda x_a,\lambda y_a)$  
+ $\overrightarrow{a}\cdot\overrightarrow{b}=x_ax_b+y_ay_b$  
+ $\overrightarrow{a}\oplus\overrightarrow{b}=x_ay_b-x_by_a$  

