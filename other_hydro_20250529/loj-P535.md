## ��Ŀ����

> ��Hanabi, hanabi������
>
> һ��˵������û���̻�Karen һ����ɥ��
>
> ���е�Ŷ���� ��Ȼ�Ȳ��ϴ����̻������ˡ���
>
> ���� Shinobu ����׼����Alice��Ayaya��Karen��Shinobu��Yoko �������ܼ���������ˣ����
>
> ���ޡ����������з�������̻����Karen �˷ܵغ�����
>
> �����ȵȡ�����Yoko ������Karen �ֳֵ�ȼ���ŵ��̻������ţ�����
>
> Yoko ��ϣ���������������������̻𣬵�Ȼ����Ź�������ᡭ�� ����ʱ���ƺ��Ѿ������ˡ�

$n$ ���̻��ų�һ�ţ������Ҹ߶ȷֱ�Ϊ $h_1,h_2,\cdots,h_n$����Щ�߶�������ͬ��

ÿ�� Yoko ����ѡ���������ڵ��̻𽻻��������Ľ������Խ��������Ρ�

ÿ�� Yoko ������ѡ�����������ڵ��̻𽻻����������Ľ����������һ�Ρ�

��������ǰ��� Yoko �����ٴ����Ľ�����ʹ��Щ�̻�����ҵĸ߶ȵ�����

## �����ʽ

��һ�а���һ�������� $n$��

�ڶ��а��� $n$ �������� $h_1,h_2,\cdots,h_n$����������֮����һ���ո������

## �����ʽ

���һ����������ʾ���ٵĽ���������

```input1
5
3 5 4 1 2
```

```output1
5
```

## ���ݷ�Χ����ʾ

�����������ݣ����� $1\le n\le 300,000$��$1\le h_i\le n$��$h_i$ ������ͬ��

<!-- BEGIN: Migrated markdown table -->

| Subtask # | ��ֵ | $n$ |
|:-:|:-:|:-:|
| 1 | $6$ | $\le 4$ |
| 2 | $11$ | $\le 8$ |
| 3 | $16$ | $\le 100$ |
| 4 | $8$ | $\le 300$ |
| 5 | $13$ | $\le 700$ |
| 6 | $7$ | $\le 2,000$ |
| 7 | $6$ | $\le 6,000$ |
| 8 | $14$ | $\le 60,000$ |
| 9 | $19$ | $\le 300,000$ |

<!-- Migrated from original HTML table:
<table class='ui table'>
    <thead>
        <tr>
            <th style='text-align: center'>Subtask #</th>
            <th style='text-align: center'> ��ֵ </th>
            <th style='text-align: center'> $n$ </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>1</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $6$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 4$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>2</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $11$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 8$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>3</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $16$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 100$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>4</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $8$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 300$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>5</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $13$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 700$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>6</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $7$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 2,000$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>7</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $6$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 6,000$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>8</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $14$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 60,000$ </td>
        </tr>
        <tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>9</td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $19$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 300,000$ </td>
        </tr>
    </tbody>
</table>
-->

<!-- END: Migrated markdown table -->

