## ��Ŀ����

T ����һ�����γ��У����� $n$ ������� $m$ ����·�����о�����Ϊ $1,2,...,n$��ÿ����·������ $n$ �������е�ĳ������������·��**����ͨ��**�ġ�ÿ����·����һ�����ȡ�

Ϊ�˷������Σ�ÿ�����㶼��һ������վ���� $i$ ������ļ���վ�ķ���Ϊ $p_i$��������Ϊ $c_i$���������ڵ� $i$ ��������ͣ�����Ҫ���� $p_i$ ԪǮ��֮�󳵵�������**������**���������� $c_i$ �еĽ�Сֵ�������������ǰ���������Ѿ���С�� $c_i$�������ڸþ�����͡�

С C ׼������ T �����Ρ�����������������Ϊ $C$�����ο�ʼʱ������������Ϊ $0$�������ι����У�

1���������������� $0$ ʱ�����������شӵ�ǰ��������������һ����·**����**��һ�����㣨����ֻ�ߵ�·��һ���֣����������������� $1$��

2���������ھ��� $i$ �ҵ�ǰ����С�� $c_i$ ʱ�����������ڵ�ǰ������ͣ������軨�� $p_i$ ԪǮ������������������Ϊ $\min\{c_i,C\}$��

һ�����ε��ܻ��ѵ���ÿ�μ��͵Ļ���֮�ͣ����ε���·�̵���ÿ�ξ�����·�ĳ���֮�͡�ע������ͬһ������ͣ�����ҲҪ�����Σ�ͬ���أ���ξ���ͬһ����·��·��ҲҪ�����Ρ�

С C �ƻ����� $T$ �Σ�ÿ������ǰ��С C ��ָ���˸ô����ε�����Ŀ��·�̡������г̲�ͬ��ÿ�γ���ǰ����ǮҲ��ͬ��Ϊ��ʡǮ��С C ��Ҫ������ǰ�ȹ滮������·�ߣ��������ε�·���ͼ��͵ķ�������ʹ�ô������������ո�����·�����ν�������·�̲�С��Ŀ��·�̣���ʣ�µ�Ǯ�����ܶࡣ����滮��������·�ߣ������� $T$ ������ÿ�ν�����������ʣ�¶���Ǯ��

## �����ʽ

�����һ�а����ĸ������� $n$��$m$��$C$��$T$��ÿ��������֮����һ���ո�������ֱ��ʾ����������·���������������޺����д�����

������ $n$ �У�ÿ�а������������� $p_i$��$c_i$��ÿ��������֮����һ���ո�����������˳�����α�ʾ���Ϊ $1,2,...,n$ �ľ���ķ��ú�������

������ $m$ �У�ÿ�а������������� $a_i$��$b_i$��$l_i$��ÿ��������֮����һ���ո��������ʾһ���ӱ��Ϊ $a_i$ �ľ��㵽���Ϊ $b_i$ �ľ���ĵ�·����·�ĳ���Ϊ $l_i$����֤ $a_i\ne b_i$������һ�����㵽��һ����������ж�����·��

��� $T$ �У�ÿ�а������������� $s_i$��$q_i$��$d_i$������һ�����μƻ������ε����Ϊ���Ϊ $s_i$ �ľ��㣬����ʱ���� $q_i$ ԪǮ��Ŀ��·��Ϊ $d_i$��

## �����ʽ

��� $T$ �У�ÿ��һ���������� $i$ �е�������ʾ�� $i$ �����ν��������ʣ�¶���ԪǮ����������޷���ɣ�Ҳ����˵�����ڴӾ��� $s_i$ �����ò����� $q_i$ ԪǮ������С�� $d_i$ ��·�̵�·�ߣ��������� $-1$��

```input1
6 6 3 2
4 1
6 2
2 1
8 1
5 4
9 1
1 2 1
1 3 1
2 4 1
3 5 1
4 6 1
5 6 1
1 12 3
1 9 3
```

```output1
2
-1
```

## ���ݷ�Χ����ʾ

���в������ݵķ�Χ���ص����±���ʾ��

<!-- BEGIN: Migrated markdown table -->

| ���Ե��� | $n$ | $m$ | $C$ | $T$ | $p_i, \ c_i$ | �������� |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| 1 | $\le 10$ | $=n-1$ | $\le 10$ | $=1$ | $\le 10$ | 1, 2 |
| 2 | $\le 10$ | $=n-1$ | $\le 10$ | $\le 10$ | $\le 10$ | 1, 2 |
| 3 | $\le 10$ | $=n-1$ | $\le 10$ | $\le 10$ | $\le 10$ | 1, 2 |
| 4 | $\le 10$ | $=n-1$ | $\le 10$ | $\le 10$ | $\le 10$ | 1, 2 |
| 5 | $=10$ | $=10$ | $\le 10$ | $\le 10$ | $\le 10$ | 2 |
| 6 | $=15$ | $=15$ | $\le 10$ | $\le 20$ | $\le 10$ | 2 |
| 7 | $=20$ | $=20$ | $\le 10$ | $\le 20$ | $\le 10$ | 2 |
| 8 | $\le 100$ | $=n-1$ | $\le 10^3$ | $\le 50$ | $\le 100$ | 1, 3 |
| 9 | $\le 100$ | $=n-1$ | $\le 10^3$ | $\le 50$ | $\le 100$ | 1, 3 |
| 10 | $\le 100$ | $=n-1$ | $\le 10^3$ | $\le 50$ | $\le 100$ | 1, 3 |
| 11 | $\le 40$ | $\le 400$ | $\le 10^3$ | $\le 50$ | $\le 100$ | 3 |
| 12 | $\le 40$ | $\le 400$ | $\le 10^3$ | $\le 50$ | $\le 100$ | 3 |
| 13 | $\le 60$ | $\le 600$ | $\le 10^3$ | $\le 50$ | $\le 10^3$ | �� |
| 14 | $\le 60$ | $\le 600$ | $\le 10^3$ | $\le 50$ | $\le 10^3$ | �� |
| 15 | $\le 80$ | $\le 800$ | $\le 10^3$ | $\le 50$ | $\le 10^3$ | �� |
| 16 | $\le 80$ | $\le 800$ | $\le 10^5$ | $\le 10^3$ | $\le 10^5$ | �� |
| 17 | $\le 90$ | $\le 900$ | $\le 10^5$ | $\le 10^3$ | $\le 10^5$ | �� |
| 18 | $\le 90$ | $\le 900$ | $\le 10^5$ | $\le 10^3$ | $\le 10^5$ | �� |
| 19 | $\le 100$ | $\le 1000$ | $\le 10^5$ | $\le 10^3$ | $\le 10^5$ | �� |
| 20 | $\le 100$ | $\le 1000$ | $\le 10^5$ | $\le 10^5$ | $\le 10^5$ | �� |

<!-- Migrated from original HTML table:
<table class='ui table'>
    <thead>
        <tr>
            <th style='text-align: center'> ���Ե��� </th>
            <th style='text-align: center'> $n$ </th>
            <th style='text-align: center'> $m$ </th>
            <th style='text-align: center'> $C$ </th>
            <th style='text-align: center'> $T$ </th>
            <th style='text-align: center'> $p_i, \ c_i$ </th>
            <th style='text-align: center'> �������� </th>
        </tr>
    </thead>
    <tbody>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 1 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='4'> $\le 10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='4'> $=n-1$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='7'> $\le 10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $=1$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='7'> $\le 10$ </td>
            <td style='text-align: center' rowspan='4'> 1, 2 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 2 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='4'> $\le 10$ </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 3 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 4 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 5 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $=10$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $=10$ </td>
            <td style='text-align: center' rowspan='3'> 2 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 6 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $=15$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $=15$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 20$ </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 7 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $=20$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $=20$ </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 8 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> $\le 100$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> $=n-1$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='8'> $\le 10^3$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='8'> $\le 50$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='5'> $\le 100$ </td>
            <td style='text-align: center' rowspan='3'> 1, 3 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 9 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 10 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 11 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 40$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 400$ </td>
            <td style='text-align: center' rowspan='2'> 3 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 12 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 13 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 60$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 600$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> $\le 10^3$ </td>
            <td style='text-align: center' rowspan='8'> �� </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 14 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 15 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 80$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 800$ </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 16 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='5'> $\le 10^5$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='4'> $\le 10^3$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='5'> $\le 10^5$ </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 17 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 90$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 900$ </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 18 </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 19 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 100$ </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 1000$ </td>
    	</tr>
    	<tr>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> 20 </td>
            <td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 10^5$ </td>
    	</tr>
    </tbody>
</table>
-->

<!-- END: Migrated markdown table -->

���У����������ʡ�һ���е������������£�

* �������� 1������ $a_i=i$��$b_i=i+1$��$l_i=1$��

* �������� 2������ $d_i\le 10^3$��

* �������� 3������ $q_i\le 100$��

�����������ݣ�$2\le n\le 100$��$1\le m\le 1000$��$1\le C,T\le 10^5$��$1\le a_i,b_i,l_i\le n$��$1\le p_i,c_i\le 10^5$��$1\le s_i\le n$��$1\le q_i\le n^2$��$1\le d_i\le 10^9$��

