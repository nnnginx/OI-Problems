## ��Ŀ����
Mirko �����о�һ����ϣ������ 

## ��Ŀ����
�˹�ϣ������˶��壺

- $f(\rm{NULL})=0$
- $f(a_i+s_i)=((f(s_i)\times33)\operatorname{xor}\ \operatorname{ord}(a_i))\bmod MOD$

���� $a_i$ ����һ���ַ���$s_i$ ����һ���ַ���������Сд��ĸ��ɡ�

- $\operatorname{xor}$ ����λ��������
- $\operatorname{ord(letter)}$ ������ĸ����ĸ���������磺$\operatorname{ord(a)=1}$��$\operatorname{ord(z)= 26}$����

$MOD$ �� $2^m$ ��ʽ��������

�� $m=10$ ʱ����ϣ������һЩֵ���£�

- $f(\texttt{a})=1$
- $f(\texttt{aa})=32$
- $f(\texttt{kit})=438$

�����ж��ٸ����ʵĹ�ϣֵΪ $k$ �ҳ���Ϊ $n$��

## �����ʽ
����һ�У������������� $n$��$k$ �� $m$��

## �����ʽ
���һ�У���ϣֵΪ $k$ �ҳ���Ϊ $n$ �ĵ��ʸ�����

```input1
1 0 10 
```

```output1
0
```

```input2
1 2 10
```

```output2
1
```

```input3
3 16 10
```

```output3
4
```

## ��ʾ
#### ���������͡�
#### ���� 1 ����
��ĸ���е������ַ��� $\text{ord}$ ֵ����Ϊ $0$��
#### ���� 2 ����
����`b`��
#### ���� 3 ����
����Ϊ`dxl`��`hph`��`lxd` �� `xpx`��

#### �����ݹ�ģ��Լ����
$1\le n\le 10$��$0\le k<2^m$��$6\le m\le 25$��

#### ��˵����
**��Ŀ���� [COCI2013-2014](https://hsin.hr/coci/archive/2013_2014/) [CONTEST #6](https://hsin.hr/coci/archive/2013_2014/contest6_tasks.pdf)  _T5 HASH_��**

