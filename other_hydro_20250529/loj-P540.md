## ��Ŀ����

С L �ƻ����� $n$ ����Ϸ��ÿ����Ϸʹ��һ�ŵ�ͼ��С L ��ͬʱʹ���������ڸõ�ͼ�������Ϸ��

С L ���������������ֱ��ô�д��ĸ A��B��C ��ʾ����ͼ��һ�������ͼ��û���ر߻��Ի�����ÿ�������ڵ�ͼ��ѡ��ͬ�������� $i$��$j$��$k$������ $i<j<k$��������֮����бߡ���ʱ������ A �� $i$ �� $j$ ��B �� $j$ �� $k$��C �� $k$ �� $i$�����һ����Ϸ�����ǵ���һ�ŵ�ͼʹ����ǡ������� $n$ ����ͬ����Ϸ���������ͼ������������ $500$����������ҵ����ŵ�ͼ��

��ʱ��С $L$ ��ǵõ�ͼ��һЩ�ص㣬�������Щ�������԰������ҵ���ͼ��

Ҳ����˵����һ�������� $n$�����㹹��һ�������ͼʹ������Ԫ������Ϊ $n$��

## �����ʽ

�����һ��һ�������� $n$��

## �����ʽ

�����һ��һ�������� $x$ ��ʾ��ͼ�е�ĸ��������� $1\le x\le 500$��  
������������ҵ��ĵ�ͼ���������ڽӾ��󡣾�����˵��ʽ���£�  
�ⲿ��һ����� $x-1$ �У����е� $i$ �й� $x-i$ �������� $i$ �е� $j$ ������ʾ�� $i$ �͵� $i+j$ �Ƿ��бߣ�ֻ��Ϊ $0$ �� $1$��Ϊ $1$ ��ʾ�У�Ϊ $0$ ��ʾû�С�

����������ʱ�����Ƕ�ȡ $x$ ֮��� $\frac{x(x-1)}{2}$ ������������Ŀհ׻�����������ԡ�

```input1
3
```

```output1
5
1 0 1 0
1 1 1
0 1
1
```

## ���ݷ�Χ����ʾ

�����������ݣ�$1\le n\le 2\times 10^6$��

<!-- BEGIN: Migrated markdown table -->

| ���Ե��� | $n$ ������ | �������� |
|:-:|:-:|:-:|
| 1 | $\le 10$ | - |
| 2 | $\le 20$ | - |
| 3 | $\le 30$ | - |
| 4 | $\le 100$ | - |
| 5 | $\le 100$ | - |
| 6 | $\le 200$ | - |
| 7 | $\le 400$ | - |
| 8 | $\le 1000$ | - |
| 9 | $\le 1000$ | - |
| 10 | $\le 3000$ | - |
| 11 | $\le 10^4$ | - |
| 12 | $\le 10^4$ | - |
| 13 | $\le 3\times 10^4$ | - |
| 14 | $\le 10^5$ | - |
| 15 | $\le 3\times 10^5$ | - |
| 16 | $\le 10^6$ | $n$ ��ĳ�������������� |
| 17 | $\le 10^6$ | ����һ����ȫͼ�������� |
| 18 | $\le 10^6$ | - |
| 19 | $\le 1.5\times 10^6$ | - |
| 20 | $\le 2\times 10^6$ | - |

<!-- Migrated from original HTML table:
<table class='ui table'>
	<thead>
		<tr>
			<th style='text-align: center'> ���Ե��� </th>
			<th style='text-align: center'> $n$ ������ </th>
			<th style='text-align: center'> �������� </th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>1</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 10$ </td>
			<td style='text-align: center' rowspan='15'> - </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>2</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 20$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>3</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 30$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>4</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 100$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>5</td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>6</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 200$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>7</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 400$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>8</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 1000$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>9</td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>10</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 3000$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>11</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='2'> $\le 10^4$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>12</td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>13</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 3\times 10^4$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>14</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 10^5$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>15</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 3\times 10^5$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>16</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;' rowspan='3'> $\le 10^6$ </td>
			<td style='text-align: center'> $n$ ��ĳ�������������� </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>17</td>
			<td style='text-align: center'> ����һ����ȫͼ�������� </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>18</td>
			<td style='text-align: center' rowspan='3'> - </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>19</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 1.5\times 10^6$ </td>
		</tr>
		<tr>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'>20</td>
			<td style='text-align: center; border-right: rgba(34, 36, 38, 0.1) 1px solid;'> $\le 2\times 10^6$ </td>
		</tr>
	</tbody>
</table>
-->

<!-- END: Migrated markdown table -->

