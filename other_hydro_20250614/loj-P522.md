## ��Ŀ����

IOI �ı�����ʼ�ˡ�Jsp �� Rlc ����һ�����䣬��ʱ����������һ������������ ����

![�ڶ������ǳ�](http://img.uoj.ac/problem/241/dark.jpg)

�������Ƿ����Լ��յ���һ������ʼ���  

> �����ڿ����Ϸ����� $N$ ��ը�����������һ��ֱ������ϵ�����ᣩ�Ļ����� $i$ ��ը���������� $X_i$����ը�뾶�� $R_i$����һ��ը����ըʱ�������һ��ը������λ�� $X_j$ ���㣺
> $$
> X_i-R_i\leq X_j\leq X_i+R_i
> $$
> ��ô��ը�� $j$ Ҳ�ᱻ������
>
> �� $i$ �� $j$ ����������ϵʽ���� $i$ ��ֱ������ $j$���� $i$ ����ֱ������ $j$�������� $i$ �ᵼ�� $j$ ��ը����� $i$ �ܼ������ $j$��
>
> �ҿ��Ը������ǣ���Щը������һ�����ʣ�**������ը�� $A$ ��ֱ�ӻ��ӵ�����ը�� $B$��������ը�� $B$ һ������ֱ�ӻ��ӵ�����ը�� $A$��**
>
> �����;Ͳ��ը���ɣ���ס���������ѡ�����������Ļ����������Ӧ��֪����

�Ծ��� Jsp �� Rlc ��ʼ�˵��������飨������֮����Щ����֤ʵ�ˡ��������˻���������һ�����ʣ�

> ����ը�� $A$ �� $B$ �ġ��������롱���� $d(A,B)$ ��ʾ��Ϊ��������������������� $a_1,a_2,...,a_n$ �ĳ��ȣ�

> 1. $a_i$ ������ͬ����Ϊ $[1,N]$ �е�������
> 2. $a_i$ ��**ֱ��**���� $a_{i+1}$��
> 3. $a_1=A,a_n=B$��

> ��ô������ʿ��Ա���Ϊ���� $d(A,B)=3$��$A$ һ����ֱ������ $B$��

������һ���о���Rlc ������Ϊ��ȫ�ķ���������������ѡ�����ɸ��ؼ�ը����װ�������Ȼ�����������

��Ϊը����ĳЩ���ԣ���װ�������ը���������һ���������� $a_1,a_2,...,a_n$�������㣺

1. $a_i$ ������ͬ����Ϊ $[1,N]$ �е�������
2. $a_i$ ��**ֱ�ӻ���**���� $a_{i+1}$��

Rlc �����һ�������������װ�����İ�ȫ�̶ȵķ�����  

���ȿ��Բ��ÿ��ը��������ֵ $v_i$��  
��ô�������װ�����İ�ȫ�̶�Ϊ��$\sum_{i=1}^{n-1}F(v_{a_i},v_{a_{i+1}})$������ $F(x,y)=(x\oplus y+xy)\bmod 998244353$��$\oplus$ ��ʾ�����ư�λ���**�����а�λ�������ȼ����ڳ˷��ͼӷ�**����

��������֪�������� $[1,N]$ �е�ÿ������ $i$���������װ����������һ��ը���� $i$���� $a_n=i$������ȫ�̶�����Ƕ��١�

**���ر�ע�⣬�����д�д�� $N$ ��ʾը��������Сд $n$ ��ʾ�������е����г��ȣ����������**

## �����ʽ

��һ��һ������ $N$ ��ʾը��������  
�ڶ��� $N$ ������ $X_1,X_2,...,X_N$����ʾը�������ꡣ  
������ $N$ ������ $R_1,R_2,...,R_N$����ʾը���ı�ը�뾶��  
������ $N$ ������ $v_1,v_2,...,v_N$����ʾը��������ֵ��

## �����ʽ

��� $N$ �У�ÿ��һ���������� $i$ �б�ʾ��������һ��ը���� $i$ ʱ�����ȫ�̶ȡ�

```input1
6
-3 -2 0 2 3 4
0 1 4 1 0 1
4 1 3 4 2 0
```

```output1
19
5
0
19
33
3
```

## ���ݷ�Χ����ʾ

�����������ݣ�$1\leq N\leq 3\times 10^5,0\leq v_i<998244353,0\leq R_i\leq 10^{18},|X_i|\leq 10^{18}$��

**���ر�ע�⣬�����д�д�� $N$ ��ʾը��������Сд $n$ ��ʾ�������е����г��ȣ����������**

<!-- BEGIN: Migrated markdown table -->

| Subtask # | ��ֵ | $N$ ������ | $v$ ������ | $R$ ������ |
|:-:|:-:|:-:|:-:|:-:|
| 1 | $10$ | $1 \leq N \leq 10 $ | �� | �� |
| 2 | $10$ | $1 \leq N \leq 300$ | �� | �� |
| 3 | $10$ | $1 \leq N \leq 3000$ | �� | �� |
| 4 | $10$ | $1 \leq N \leq 3\times 10^5$ | $v_i=1$ | �� |
| 5 | $15$ | $1 \leq N \leq 3\times 10^5$ | $v_i\in\{0,1\}$ | �� |
| 6 | $15$ | $1 \leq N \leq 3\times 10^5$ | �� | $R_i\leq 10^4$ |
| 7 | $30$ | $1 \leq N \leq 3\times 10^5$ | �� | �� |

<!-- Migrated from original HTML table:
<table class='ui table'>
    <thead>
        <tr>
            <th style='text-align: center'>Subtask #</th>
            <th style='text-align: center'> ��ֵ </th>
            <th style='text-align: center'> $N$ ������ </th>
            <th style='text-align: center'> $v$ ������ </th>
            <th style='text-align: center'> $R$ ������ </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>1</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $1 \leq N \leq 10 $ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> �� </td>
            <td style='text-align: center' rowspan='5'> �� </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>2</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> $1 \leq N \leq 300$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>3</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> $1 \leq N \leq 3000$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>4</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='4'> $1 \leq N \leq 3\times 10^5$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> $v_i=1$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>5</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $15$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> $v_i\in\{0,1\}$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>6</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $15$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> �� </td>
            <td style='text-align: center' rowspan='1'> $R_i\leq 10^4$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>7</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $30$ </td>
            <td style='text-align: center' rowspan='1'> �� </td>
        </tr>
    </tbody>
</table>
-->

<!-- END: Migrated markdown table -->

