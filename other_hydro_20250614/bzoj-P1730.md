## ��Ŀ����
Farmer John has $n \ (1 \le n \le 2.5\times 10^4)$ rectangular barns on his farm, all with sides parallel to the $x$ and $y$ axes and integer corner coordinates in the range $0\dots 10^6$. These barns do not overlap although they may share corners and/or sides with other barns. Since he has extra cows to milk this year, FJ would like to expand some of his barns. A barn has room to expand if it does not share a corner or a wall with any other barn. That is, FJ can expand a barn if all four of its walls can be pushed outward by at least some amount without bumping into another barn. If two barns meet at a corner, neither barn can expand. Please determine how many barns have room to expand.


Լ���� $n$ ������ţ����ǵ�ǽ����������ƽ�У������������� $[0,10^6]$ ��Χ�ڡ���������ţ�ﲻ�ص��������ܻ��й�����ǽ������Լ������ţ�������ӣ������ò���������ţ�һ��ţ��������ţ����ҽ��������ı߾���������ţ��Ӵ����������ţ����һ�������ǣ������Ǿ��ǲ������ŵġ�ͳ���ж���ţ��������š�
## �����ʽ
* Line $1$��A single integer,$n$.
* Lines $2\dots n+1$��Four space-separated integers $a,b,c$, and $d$, describing one barn. The lower-left corner of the barn is at $\ (a,b)$ and the upper right corner is at $\ (c,d)$.

��һ������ $n$��֮�� $n$ ��ÿ������һ��ţ������½Ǻ����Ͻ����ꡣ

## �����ʽ
* Line $1$��A single integer that is the number of barns that can be expanded.

��������ŵ�ţ������
```input1
5
0 2 2 7
3 5 5 8
4 2 6 4
6 1 8 6
0 0 8 1
```
```output1
2
```
## ����˵��
INPUT DETAILS��  
There are 5 barns. The first barn has its lower-left corner at $\ (0,2)$ and its upper-right corner at $\ (2,7)$, and so on.

����ǰ����ţ��������š�

## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq n \leq 2.5\times 10^4$��
## ��Ŀ��Դ
Gold