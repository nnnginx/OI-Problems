## ��Ŀ����

> �������ĵ��������ڵ��ˡ����죬���������˱��򿼳����г���Ϧ�����ɫ����գ����Ŵ��ڵ�Ŀ���ߵļ�Ӱ����Ϊ���г���ʧǰ���ı�����
>
> �г�������ʻ��Rlc ���� Jsp��������ֹ������֪�� Jsp �� OI ����Ķ�������һ������������ӣ�����������һ�����������⣺

������ȫͼ $G=(V,E)$��ÿ���� $v\in V$ ��һ��Ȩֵ $w_v\in\mathbb{Z}$���� $e=(u,v)\in E$ �ĳ��� $w_e$ ����Ϊ $w_e=(w_u-w_v)^2$��

��Ҫ��һ�� $G$ �еĹ��ܶٻ�· $C$��Ҫ�󾭹� $V$ �еĸ�����ǡ��һ�Σ��һ�·�ĳ��� $w(C)$ ��С����· $C$ �ĳ��� $w(C)$ ����Ϊ $C$ ���������бߵĳ���֮�ͣ���

$$w(C)=\sum_{e\in E(C)}w_e$$

��ֻ�������С�� $w(C)$ ֵ��

## �����ʽ

�����һ�а���һ�������� $n$����ʾ $|V|$���� $V=\{1,2,\cdots,n\}$��

�ڶ��а��� $n$ ���ɿո�ָ�����������ʾ $w_1,w_2,\cdots,w_n$��

## �����ʽ

�����һ�У�����һ����������ʾ��С�� $w(C)$ ֵ��

```input1
4
1 2 3 4
```

```output1
10
```

## ���ݷ�Χ����ʾ

�����������ݣ����� $2\le n\le 100,000$��$-10^9\le w_v\le 10^9$��

<!-- BEGIN: Migrated markdown table -->

| Subtask # | ��ֵ | $n$ | $\|w_v\|$ |
|:-:|:-:|:-:|:-:|
| 1 | $10$ | $\le 10$ | $\le 10^3$ |
| 2 | $10$ | $\le 15$ | $\le 10^3$ |
| 3 | $10$ | $\le 20$ | $\le 10^3$ |
| 4 | $20$ | $\le 100$ | $\le 10^3$ |
| 5 | $20$ | $\le 2,000$ | $\le 10^6$ |
| 6 | $30$ | $\le 100,000$ | $\le 10^9$ |

<!-- Migrated from original HTML table:
<table class='ui table'>
    <thead>
        <tr>
            <th style='text-align: center'>Subtask #</th>
            <th style='text-align: center'> ��ֵ </th>
            <th style='text-align: center'> $n$ </th>
            <th style='text-align: center'> $|w_v|$ </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>1</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='4'> $\le 10^3$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>2</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 15$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>3</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 20$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>4</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $20$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 100$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>5</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $20$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 2,000$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 10^6$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>6</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $30$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 100,000$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 10^9$ </td>
        </tr>
    </tbody>
</table>
-->

<!-- END: Migrated markdown table -->

