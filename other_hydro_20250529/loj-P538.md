## ��Ŀ����

sosusosu Ű�� OI ֮���Ϊ��һ���Ļ���ѡ�֡�һ�죬������ҵ������һ���������⣬ÿ������������ж���������ʽ��

> ����һ���±�� $0$ ��ʼ�����޳��������� $\{a_i\},\ i\in \mathbb{N}$����֪ $a_0,a_1$ ��ֵ���Լ�����ʽ $a_{i+2}=k a_{i+1}+a_i,\ i\in\mathbb{N},k\in {\mathbb{N}^+}$��

sosusosu �о�����Щ���У���������ʮ���������������ǻۣ����Ǿ�����һ�� OI �⡣

sosusosu ������һ������ $S\subset \mathbb{N}$������������� $S$ �е�ÿ���� $s_i$��ʹ�� $a_{s_i}$ ���� $s_i$ ��ʹ�� $a_{s_i}$ ��С�� $s_i$ �ֱ��Ƕ��١���������� $s_i$ �ж��������ش���С��һ����

���⣬sosusosu ׼��������ҵ��������ÿ�����ж�����ش�һ�Σ�����ÿ�εļ��� $S$ ��һ���ġ�

## �����ʽ

�����һ��һ������ $m$ ��ʾ $S$ ��Ԫ�ظ�����  
�ڶ��� $m$ ������ $s_1,s_2,\cdots ,s_m$ ��ʾ $S$ �е�Ԫ�ء���֤�����ǷǸ��������ϸ�������� $s_i<s_{i+1}$����  
������һ������ $n$ ��ʾѯ�ʵ����и�����  
������ $n$ ��ÿ���������� $a_0, a_1, k$ ����һ�����С�

## �����ʽ

����� $n$ �У�ÿ����������������� $\mathrm{maxsi},\mathrm{minsi}$�����α�ʾ $S$ ��Ԫ�� $s_i$ �У�ʹ�� $a_{s_i}$ ���� $s_i$ ��ʹ�� $a_{s_i}$ ��С�� $s_i$ ��ֵ����������� $s_i$ �ж��������ش���С��һ����

```input1
8
1 2 3 4 5 6 7 8
2
10 -6 1
0 0 1
```

```output1
2 1
1 1
```

```input2
3
0 1 2
2
-2 3 1
3 -2 2
```

```output2
1 0
0 1
```

```input3
29
2 4 8 16 32 64 128 256 512 1024 2048 4096 8192 16384 32768 65536 131072 262144 524288 1048576 2097152 4194304 8388608 16777216 33554432 67108864 134217728 268435456 536870912
4
10000000 10000000 100
9999984 -6180330 1
9999984 -6180329 1
-10000000 4142135 2
```

```output3
536870912 2
2 536870912
536870912 16
8 536870912
```

## ���ݷ�Χ����ʾ

�����������ݣ�$1\le n\le 3\times 10^5$��$1\le m\le 10^5$��$0\le s_i\le 10^9$��$-10^7\le a_0,a_1\le 10^7$��$1\le k\le 5\times 10^3$����֤ $s_i$ �ϸ񵥵�������

**ע�⣬���������ģ�ϴ���ʹ�ýϿ�ķ�ʽ���롣LOJ �� C ���Ե� `scanf`��C++ ��[�ر�ͬ��](http://en.cppreference.com/w/cpp/io/ios_base/sync_with_stdio)�� `cin`��Pascal �� `read` �����������ʱ����� 50 ~ 200 ����֮�䡣**

���в������ݵķ�Χ���ص����±���ʾ��  
��δ�������������������ݵ�����Ϊ׼��
<!-- BEGIN: Migrated markdown table -->

| ���Ե��� | $n,m$ ������ | $a_0,a_1,k$ �ķ�Χ | �������� |
|:-:|:-:|:-:|:-:|
| 1 | $n,m\le 100$ | $-100\le a_0,a_1\le 100,k\le 10$ | $s_m\le 10$ |
| 2 | $n,m\le 100$ | $-100\le a_0,a_1\le 100,k\le 10$ | $s_m\le 10$ |
| 3 | $n,m\le 100$ | $-100\le a_0,a_1\le 100,k\le 10$ | $s_m\le 10$ |
| 4 | $n\le 10^5$ | $k=1$ | - |
| 5 | $n\le 10^5$ | $k=1$ | - |
| 6 | $n\le 10^5$ | $k=1$ | - |
| 7 | $n\le 10^5$ | - | $a_0\cdot a_1\ge 0$���� $a_0,a_1$ ����һ��һ���� |
| 8 | $n\le 10^5$ | - | $\|a_1\|\ge\|a_0\|$ |
| 9 | $n\le 10^5$ | - | $S$ ��Ԫ�ض���ż�� |
| 10 | $n\le 10^5$ | - | $S$ ��Ԫ�ض���ż�� |
| 11 | $n\le 10^5$ | - | $S$ ��Ԫ�ض���ż�� |
| 12 | $n\le 10^5$ | $k\le 10$ | $S$ ��Ԫ�ض���ż�� |
| 13 | $n\le 10^5$ | $k\le 100$ | $S$ ��Ԫ�ض���ż�� |
| 14 | $n\le 10^5$ | $k\le 1000$ | - |
| 15 | $n\le 10^5$ | - | - |
| 16 | $n\le 1.5\times 10^5$ | $k\le 10$ | - |
| 17 | $n\le 2\times 10^5$ | $k\le 100$ | - |
| 18 | $n\le 2.5\times 10^5$ | $k\le 1000$ | - |
| 19 | - | - | - |
| 20 | - | - | - |

<!-- Migrated from original HTML table:
<table class='ui table'>
	<thead>
		<tr>
			<th style='text-align: center'> ���Ե��� </th>
			<th style='text-align: center'> $n,m$ ������ </th>
			<th style='text-align: center'> $a_0,a_1,k$ �ķ�Χ </th>
			<th style='text-align: center'> �������� </th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>1</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> $n,m\le 100$ </td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> $-100\le a_0,a_1\le 100,k\le 10$ </td>
			<td style='text-align: center' rowspan='3'> $s_m\le 10$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>2</td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>3</td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>4</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='12'> $n\le 10^5$ </td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> $k=1$ </td>
			<td style='text-align: center' rowspan='3'> - </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>5</td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>6</td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>7</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='5'> - </td>
			<td style='text-align: center'> $a_0\cdot a_1\ge 0$���� $a_0,a_1$ ����һ��һ���� </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>8</td>
			<td style='text-align: center'> $|a_1|\ge|a_0|$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>9</td>
			<td style='text-align: center' rowspan='5'> $S$ ��Ԫ�ض���ż�� </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>10</td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>11</td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>12</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $k\le 10$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>13</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $k\le 100$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>14</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $k\le 1000$ </td>
			<td style='text-align: center' rowspan='7'> - </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>15</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> - </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>16</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $n\le 1.5\times 10^5$ </td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $k\le 10$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>17</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $n\le 2\times 10^5$ </td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $k\le 100$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>18</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $n\le 2.5\times 10^5$ </td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $k\le 1000$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>19</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> - </td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> - </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>20</td>
		</tr>
	</tbody>
</table>
-->

<!-- END: Migrated markdown table -->

