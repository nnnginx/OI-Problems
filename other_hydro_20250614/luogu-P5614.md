## ��Ŀ����
��ǿ����ǿ��$\mathsf S\mathsf{\color{red} iyuan}$ ����ǿ������$\mathsf S \mathsf{\color{red} iyuan}$

disangan233 ���������һ�� OIer �ǵ���Ϸ��[Ĥ $\color{black} \mathsf S \mathsf{\color{red} iyuan}$](https://lmoliver.github.io/mosiyuan/index.html)��

��������ġ����� IV���������������ҵ�����Ѱ�������


## ��Ŀ����
���� $1$ �������� $M$��$n(n\leq 5)$ �������� $3$ Ԫ�� $\{a_i,b_i,c_i\}(a_i,b_i,c_i\leq M\leq 2000)$�����������������

$$
\forall i\leq n ,s.t.~|a_i-x|\oplus |b_i-y|\oplus |c_i-z| = 9
$$

��**����**������ $3$ Ԫ�� $\{x,y,z\}(x,y,z \leq M)$�ĸ�����

���У�$\forall$ ��ʾ "��������"��$s.t.$ ��ʾ "ʹ��"��$A \oplus B \oplus C$ ��ʾ $A,B,C$ �����͡�

���� C++��`A^B^C` �� `A xor B xor C` ��Ϊ $A \oplus B \oplus C$ �Ĵ� ��

�����ṩһ��ģ�壺

```cpp
if ((a ^ b ^ c) == 9) 
{
	Your code here...
}
```

���� $2$ ������ $3$ Ԫ�� $A,B$����� $x_A \not =x_B$ �� $y_A \not =y_B$ �� $z_A \not =z_B$��$A,B$ ������Ϊ�ǲ�ͬ�ġ�


## �����ʽ
�� $n+1$ �С�

�� $1$ ������ $2$ �������� $n$��$M$��

������ $n$ �е� $i$ ������ $3$ �������� $a_i,b_i,c_i$��

## �����ʽ
�� $1$ �У���� $1$ ���Ǹ�������ʾ����𰸡�

```input1
5 200
21 84 198
38 47 102
44 47 132 
63 150 166
76 79 132
```

```output1
4
```

## ��ʾ
#### �������� $1$

�������������� $\{x,y,z\}$ �У� 

$\{88,88,120\}$��$\{88,104,104\}$��$\{120,120,120\}$ �� $\{120,136,104\}$��

�� $4$ ����

### ������

���� $10\%$ �����ݣ���֤��������ȫһ�¡�

���� $60\%$ �����ݣ���֤ $M\leq 200$��

�����������ݣ���֤ $a_i,b_i,c_i\leq M\leq 2000$��$n\leq 5$��


### ��Ŀ��Դ

[MtOI2019 Extra Round](https://www.luogu.org/contest/22614) T2

�����ˣ�disangan233

�����ˣ�Studying Father


