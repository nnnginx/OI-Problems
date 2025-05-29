## ��Ŀ����

����������δ����ͨ����չ�����Ϲ�����һ����$m$ ѭ�����������ֽ�ͨ���ߵ��ص��ǣ�����ÿ��ʻ $m$ �ײ��ܿ���һ�Ρ�

չ���������׼���ؼң�Ȼ������Կ�׺󣬳��ڵ�һ��ͻȻŤ�������� ���� �����������Լ�����һ����ֵĵط�����ʱ���д���һ��������
  
> ������ ���� �����������������Ϊ�˿���һ�����ǵ�ˮƽ�����������һ������ͼ���� $n$ ���㣬��ʱ��û�бߡ���һ���Ұѱ߼���֮��ÿ���߻���һ�����ȣ��� $i$ ���߳� $w_i$ �ס�  
> ���ǵĳ�һ��ʻ��һ���ߣ��ͱ��뿪�������ߵľ�ͷ����;û�л�ת����ء�   
>
> �������ǽ�Ҫ���� $q$ �ο��顣���������֣�
>
> 1. ���������������� $u,v,w$ ��ʾ���� $u$ �� $v$ ֮�����һ���� $w$ �׵ıߣ�
> 2. ��������������� $u,v,x,b,c \ (u\neq v)$������ $x,b$ ������һ��α�����������������һ�εķ���ֵ $f_1=x\bmod m$���Ժ�ÿ�εķ���ֵ $f_{i+1}=(f_i+b)\bmod m$������Ҫ�ش𣬶��� $i=1,2,\ldots,c$���ж��ٸ� $i$ ���㣺�����ĳ������һ���ܹ����ŵĻ��ỹ�� $f_i$ �ף���ô����һ��·��ʹ���ܴ� $u$ ������ $v$ �³���
>
> �������ǵĻش�ȫ����ȷ�ҿ��٣��������ǲ���������뿪����� ���� ������ ����  

������·�������Ȼ��һ�������������⡣����Ϊ�˲��úڶ������װ׳�������������Ҳ���һ��������⡣

<hr/>

**��������**��һ������Ȩ����ͼ�������ֲ������ӱ��Լ�ѯ���� $x,x+b,...,x+(c-1)b$ ��Щ���У��ж��ٴ���һ����֮ģ $m$ ͬ��Ĵ� $u$ �� $v$ ��·�������Բ��Ǽ�·������


## �����ʽ

��һ���������� $n,m,q$��  
������ $q$ �У�ÿ������һ�ο��飬�������£�

* $\texttt{1 u v w}$ ��ʾ $u$ �� $v$ ֮�����һ���� $w$ �׵ıߣ�
* $\texttt{2 u v x b c}$ ��ʾѯ�ʶ��� $i=1,2,\ldots,c$���ж��ٸ� $i$ ���㣺�����ĳ������һ���ܹ����ŵĻ��ỹ�� $f_i$ �ף���ô����һ��·��ʹ���ܴ� $u$ ������ $v$ �³���

## �����ʽ

����ÿ���ڶ��ֿ��飬���һ��һ��������ʾ�𰸡�

```input1
6 6 10
1 1 2 3
2 1 2 0 0 1
1 2 3 3
1 1 3 3
2 1 2 0 0 1
1 4 5 6
1 5 6 4
2 4 6 2 0 1
1 3 4 6
2 1 6 0 1 6
```

```output1
0
1
1
6
```

## ���ݷ�Χ����ʾ

���� $100\%$ �����ݣ�$1\leq n,q\leq 10^6,1< m\leq 10^9,1\leq w\leq m,0\leq x,b< m,1\leq c\leq 10^9$��**���� 2 �б�֤ $u\neq v$**��

���������һ���ܹ����ŵĻ��ỹ�� $r$ ��ʱ��������һ��·��ʹ���ܴ� $u$ ������ $v$ �³�������˼�� $u$ �� $v$ ֮�����һ��·�������Բ��Ǽ�·��������ģ $m$ Ϊ $r$�� 

**ע�⣬·�����Բ��Ǽ�·����**

**�����˵Ĺػ������������ģ�ϴ󣬽���ʹ�ö����Ż��������� LibreOJ ���������ٶȡ�**

<!-- BEGIN: Migrated markdown table -->

| Subtask # | ��ֵ | $n, q$ ������ | $m$ ������ | $c$ ������ | �������� |
|:-:|:-:|:-:|:-:|:-:|:-:|
| 1 | $11$ | $1 \leq n, q \leq 100 $ | $1 < m \leq 100 $ | $1 \leq c \leq 5 $ | �� |
| 2 | $21$ | $1 \leq n, q \leq 2\times 10^5$ | $m=2 $ | $1 \leq c \leq 5 $ | �� |
| 3 | $13$ | $1 \leq n, q \leq 2\times 10^5$ | $m$ ������ | $1 \leq c \leq 5 $ | �� |
| 4 | $7$ | $1 \leq n, q \leq 2\times 10^5$ | $m$ ������ | $1 \leq c \leq 5 $ | ͼ���κ�ʱ�̶�������ּ򵥻� |
| 5 | $10$ | $1 \leq n, q \leq 2\times 10^5$ | $m$ ������ | �� | �� |
| 6 | $5$ | $1 \leq n, q \leq 2\times 10^5$ | �� | $1 \leq c \leq 5 $ | ͼ���κ�ʱ�̲����ж������� $2$ �ĵ� |
| 7 | $13$ | $1 \leq n, q \leq 2\times 10^5$ | �� | $1 \leq c \leq 5 $ | �� |
| 8 | $20$ | $1 \leq n, q \leq 10^6 $ | �� | �� | �� |

<!-- Migrated from original HTML table:
<table class='ui table'>
    <thead>
        <tr>
            <th style='text-align: center'>Subtask #</th>
            <th style='text-align: center'> ��ֵ </th>
            <th style='text-align: center'> $n, q$ ������ </th>
            <th style='text-align: center'> $m$ ������ </th>
            <th style='text-align: center'> $c$ ������ </th>
            <th style='text-align: center'>��������</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>1</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $11$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $1 \leq n, q \leq 100 $ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $1 < m \leq 100 $ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='4'> $1 \leq c \leq 5 $ </td>
            <td style='text-align: center' rowspan='3'>��</td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>2</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $21$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='6'> $1 \leq n, q \leq 2\times 10^5$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> $m=2 $ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>3</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $13$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> $m$ ������ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>4</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $7$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $m$ ������ </td>
            <td style='text-align: center' rowspan='1'> ͼ���κ�ʱ�̶�������ּ򵥻� </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>5</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> �� </td>
            <td style='text-align: center' > �� </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>6</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $5$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> �� </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $1 \leq c \leq 5 $ </td>
            <td style='text-align: center' rowspan='1'> ͼ���κ�ʱ�̲����ж������� $2$ �ĵ� </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>7</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $13$ </td>
            <td style='text-align: center' rowspan='2'> �� </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>8</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $20$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> $1 \leq n, q \leq 10^6 $ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> �� </td>
        </tr>
    </tbody>
</table>
-->

<!-- END: Migrated markdown table -->

