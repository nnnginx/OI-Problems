## ��Ŀ����

�ص���������ʱ�գ���ĺ� LCR ��ʱ���Ű�����ƽ����������ǻ���������ǰ�����¡���

> ���յı�У�Ÿ������������죬��ĺ� LCR ��һ����ѧ�ж�����������

����������������ǣ����� LCR ��������У��������¡��ǿ�����������̬����ӡ����ĵ����С���ĳ��������һ�á�K ��������  
Ϊ�˼������� LCR �ĵ�һ����������ĺ���д����״���鶼���� K ���ƶ��Ƕ�����Ϊ���ġ�

��ĵĻ�������һλ���� LCA ���X�m��һ�����������͵�����ĵĴ��룬��������ĵ���״��������ôд�ģ�  

```
function add(x,v)
    while x <= n do
        s[x] = s[x] xor v
        x = x + lowbitv(x)
    end while
end function

function query(x)
    ans = 0
    while x > 0 do
        ans = ans xor s[x]
        x = x - lowbit(x)
    end while
    return ans
end function
```
���У�
* $\mathrm{lowbit}(x)$ ��ʾ $K$ ������ $x$ ����ͷ���λ��ֵ�����統 $K=5$ ʱ��$\mathrm{lowbit}(230_{(5)})=30_{(5)}=15_{(10)}$��
* $\mathrm{lowbitv}(x)$ ��ʾ $K$ ������ $x$ ����ͷ���λ��λֵ������λΪ 1 ����λ��Ϊ 0 ʱ����ֵ�����統 $K=5$ ʱ��$\mathrm{lowbitv}(230_{(5)})=10_{(5)}=5_{(10)}$��

��ݴ����������ά��һ������Ϊ $n$ ������ $A$��֧�ֵ���**���**��һ��ֵ����ǰ׺**����**��$s[i]$ ά������ $\mathop{\oplus}\limits_{i\in (s[i]-\mathrm{lowbit}(s[i]),s[i]]} A_i$����$\oplus$ ��ʾ��λ���

LCA ��������д��ʮ�ֲ��������Լ�Ҳ��ôд��������д�ҵ� LCA ©����һ���ַ������� $K$ ��ֵ�趨�ô��˺ܶࡣ

Ҳ����˵��LCA �Ĵ�������ôд�ģ�
```
function add(x,v)
    while x <= n do
        s[x] = s[x] xor v
        x = x + lowbit(x) //ע�⣬������ lowbit����Ҳ�����ݴ���Ψһ������
    end while
end function

function query(x)
    ans = 0
    while x > 0 do
        ans = ans xor s[x]
        x = x - lowbit(x)
    end while
    return ans
end function
```
**ע�⣺�����������õĶ��� $\mathrm{lowbit}$��**

������ LCA �ͷ����Լ��Ĵ����ܵñ�˭����������˼������⣬ֻ��������������������⡣

��дһ���� LCA �ĳ���������ͬ�ĳ���

**ע�⣬���������дһ���� LCA �ĳ��������ͬ�ĳ��򣬶�������ȷ�ĳ���**

## �����ʽ

��һ������������ $n,q,K$����ʾ���г��ȣ��������ͽ��ƵĻ�����**���г�ʼȫΪ 0��LCA �� s ����Ҳ���ʼ��Ϊȫ 0**��  
������ $q$ ��ÿ�и�ʽ������֮һ��  
* $\texttt{1 x v}$ �� $A_x$ ��ֵ����� $v$��LCA ����� $\mathrm{add}(x,v)$��
* $\texttt{2 x}$ ��ѯ $\mathop{\oplus}\limits_{i\in (0,x]} A_i$��LCA �����һ��һ��������Ϊ���� $\mathrm{query}(x)$ �Ľ����


## �����ʽ

����ÿ�� 2 ���������һ��������ʾ **LCA ��������**��

**ע�⣬���������дһ���� LCA �ĳ��������ͬ�ĳ��򣬶�������ȷ�ĳ���**

```input1
7 16 5
1 1 10
2 1
1 4 15
2 4
1 6 10
1 4 15
2 6
2 6
1 6 5
1 5 12
2 3
1 2 5
1 4 5
2 5
1 6 0
1 5 5
```

```output1
10
5
10
10
0
12
```

## ���ݷ�Χ����ʾ

���� $100\%$ �����ݣ�$1\leq x\leq n\leq 10^9,1\leq q\leq 2\times 10^5,2\leq K\leq 2\times 10^5,0\leq v\leq 10^9$��

**ע�⣬���������дһ���� LCA �ĳ��������ͬ�ĳ��򣬶�������ȷ�ĳ���**

<!-- BEGIN: Migrated markdown table -->

| Subtask # | ��ֵ | $n,q$ ������ | $K$ ������ |
|:-:|:-:|:-:|:-:|
| 1 | $17$ | $1 \leq n, q \leq 3000 $ | $2 \leq K \leq 3000 $ |
| 2 | $15$ | $1 \leq n \leq 2\times 10^5$ | $K=2 $ |
| 3 | $19$ | $1 \leq n \leq 2\times 10^5$ | $K$ ������ |
| 4 | $24$ | $1 \leq n \leq 2\times 10^5$ | �� |
| 5 | $25$ | �� | �� |

<!-- Migrated from original HTML table:
<table class='ui table'>
    <thead>
        <tr>
            <th style='text-align: center'>Subtask #</th>
            <th style='text-align: center'> ��ֵ </th>
            <th style='text-align: center'> $n,q$ ������ </th>
            <th style='text-align: center'> $K$ ������ </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>1</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $17$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $1 \leq n, q \leq 3000 $ </td>
            <td style='text-align: center'> $2 \leq K \leq 3000 $ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>2</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $15$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> $1 \leq n \leq 2\times 10^5$ </td>
            <td style='text-align: center' rowspan='1'> $K=2 $ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>3</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $19$ </td>
            <td style='text-align: center' rowspan='1'> $K$ ������ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>4</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $24$ </td>
            <td style='text-align: center' rowspan = '2'> �� </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>5</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $25$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='1'> �� </td>
        </tr>
    </tbody>
</table>
-->

<!-- END: Migrated markdown table -->

