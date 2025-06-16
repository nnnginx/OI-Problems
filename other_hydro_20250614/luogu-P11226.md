## ��Ŀ����

���� [Izborne Pripreme 2019 (Croatian IOI/CEOI Team Selection)](https://hsin.hr/pripreme2019/) D2T3��$\texttt{1.5s,0.5G}$��

## ��Ŀ����


��ĳ�� ICPC Regional �У���ί������ö��������ֵ������������������ҵ��ǣ����ڶ�������ĸ $\texttt{z}$ ��ͷ�Ķ��飬�����൱����ƽ�ġ�

�������ۣ���ί������������ȡһ�� $26$ ����ĸ�����У�����ĸ�����ж�Ӧ���ֵ���������������

�� $N$ ֧����μ����ⳡ��������������ΪСдӢ����ĸ��

Etna д��һ������ö���� $26!$ �����У������ҵ���ʹÿ�������ڵ����С����������������û���ܳ������

�������������㣬Ϊÿ�����鹹��һ�����У�ʹ����֧�����ڡ�


## �����ʽ

��һ�У�һ�������� $N$��

������ $N$ �У��� $i$ ��һ���ַ�������ʾ�� $i$ ֧����Ķ�������

��֤������������ͬ��

## �����ʽ

��� $N$ �У�
- �������ʹ����֧�����ʤ�����һ�� $26$ ����ĸ�����У�
- ������� `nemoguce`�����޵���������ܡ�����

```input1
3
war
zag
wro
```

```output1
agorwzbcdefhijklmnpqstuvxy
agorzwbcdefhijklmnpqstuvxy
gorawzbcdefhijklmnpqstuvxy
```

```input2
3
b
ab
aa
```

```output2
bacdefghijklmnopqrstuvwxyz
nemoguce
abcdefghijklmnopqrstuvwxyz
```

```input3
7
bcada
dbaab
bbabc
ababb
aacdf
bcdff
baddb
```

```output3
cbadfeghijklmnopqrstuvwxyz
cdabfeghijklmnopqrstuvwxyz
bacdfeghijklmnopqrstuvwxyz
nemoguce
abcdfeghijklmnopqrstuvwxyz
cbdafeghijklmnopqrstuvwxyz
nemoguce
```

## ��ʾ

�� $L$ Ϊ�ַ����ܳ��ȣ�$|\Sigma|$ Ϊ�ַ����ַ�����С��

���� $100\%$ �����ݣ���֤��

- $1\le N\le 25\, 000$��
- $1\le L\le 10^6$��
- ������������ͬ��
- $1\le |\Sigma|\le 26$��


| �������� | $N\le $ | $L\le $ | $\vert\Sigma\vert\le$    | �÷� |  
| :--: | :--: |:--: |  :--: | :--: | 
| $ 1 $    | $ 100 $ |   $ 10^4 $   |  $6$ | $13$ |
| $ 2 $    | $ 350 $ |  $ 10^4 $   |  $26 $ | $32$ |
| $ 3 $    | $ 25\, 000 $ | $ 10^6 $   |  $26$ |  $55$ |

