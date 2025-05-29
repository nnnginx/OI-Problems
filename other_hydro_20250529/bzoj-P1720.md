## ��Ŀ����
Farmer John wishes to build a corral for his cows. Being finicky beasts, they demand that the corral be square and that the corral contain at least $c \ (1  \leq  c  \leq  500)$ clover fields for afternoon treats. The corral's edges must be parallel to the $x,y$ axes. FJ's land contains a total of $n \ (c  \leq  n  \leq  500)$ clover fields, each a block of size $1 \times 1$ and located at with its lower left corner at integer $x$ and $y$ coordinates each in the range $1 \ldots 10^4$. Sometimes more than one clover field grows at the same location;such a field would have its location appear twice (or more) in the input. A corral surrounds a clover field if the field is entirely located inside the corral's borders. Help FJ by telling him the side length of the smallest square containing $C$ clover fields.

Լ�����㽨һ��Χ����Ȧ��������ţ����Ϊ�����޵����࣬��ţ��Ҫ�����Χ�������������εģ�����Χ��������Ҫ�� $c$ ���ݳ�������Ӧ���ǵ���͡�Լ���������Ϲ��� $n$ ���ݳ���ÿ���ݳ���һ�� $1\times1$ �ķ����ڣ����������������겻�ᳬ�� $10^4$����ʱ�򣬻��ж���ݳ���ͬһ�������ڣ������ǵ�����ͻ���ͬ������Լ������С��Χ���ı߳��Ƕ��٣�
## �����ʽ
* Line $1$��Two space-separated integers��$c$ and $n$.
* Lines $2 \ldots n+1$��Each line contains two space-separated integers that are the $x,y$ coordinates of a clover field.

�� $1$ ������ $c$ �� $n$�������� $n$ ��ÿ������һ����������ʾһ���ݳ����ڷ�������ꡣ
## �����ʽ
* Line $1$��A single line with a single integer that is length of one edge of the minimum size square that contains at least $c$ clover fields.

�����С�߳���
```input1
3 4
1 2
2 1
4 1
5 2
```
```output1
4
```
## ����˵��
Below is one $4\times 4$ solution( C's show most of the corral's area ) ; many others exist.
```
|CCCC
|CCCC
|*CCC*
|C*C*
+------
```
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq c \leq 500$��$c \leq n \leq 500$��
## ��Ŀ��Դ
Gold