## ��Ŀ����

Rain has pummeled the cows' field, a rectangular grid of $r$ rows and $c$ columns $(1 \le r, c \le  50)$. While good for the grass, the rain makes some patches of bare earth quite muddy. The cows, being meticulous grazers, don't want to get their hooves dirty while they eat. To prevent those muddy hooves, Farmer John will place a number of wooden boards over the muddy parts of the cows'field. Each of the boards is $1$ unit wide, and can be any length long. Each board must be aligned parallel to one of the sides of the field. Farmer John wishes to minimize the number of boards needed to cover the muddy spots, some of which might require more than one board to cover. The boards may not cover any grass and deprive the cows of grazing area but they can overlap each other. Compute the minimum number of boards FJ requires to cover all the mud in the field.

������Ϯ����ţ�ǵ�������������һ�� $r \times c$ �ľ��Ρ����꽫û�г��ݵ�����Ū����Ţ����������С�ĵ���ţ�ǲ����ڳԲݵ�ʱ��Ū�����ǵ����ӡ�Ϊ�˷�ֹ���ǵ����ӱ�Ū�࣬Լ����������Ţ�����������һЩľ�塣ÿһ��ľ��Ŀ��Ϊ $1$ ����λ���������⡣ÿһ������������ƽ��������������Լ����ʹ�����ٵ�ľ�帲�����е���ء�һ��ľ������ص�����һ��ľ���ϣ����ǲ��ܷ��ڲݵ��ϡ�

## �����ʽ
* Line $1$: Two space-separated integers: $r$ and $c$.
* Lines $2\dots r+1$: Each line contains a string of $c$ characters, with `*` representing a muddy patch, and `.` representing a grassy patch. No spaces are present.
* ��һ�У��������� $r$ �� $c$��
* �ڶ��� $r+1$ �У�ÿ�� $c$ ���ַ������� `*` ������أ�`.` ����ݵء�
## �����ʽ
* Line $1$��A single integer representing the number of boards FJ needs.
* ������Ҫ����ľ�塣
```input1
4 4
*.*.
.***
***.
..*.
```
```output1
4
```
## ����˵��
Boards $1,2,3$ and $4$ are placed as follows��
```
|1|.|2|.|
|.|3|3|3|
|4|4|4|.|
|.|.|2|.|
```
Board $2$ overlaps boards $3$ and $4$.
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq r,c \leq 50$��
## ��Ŀ��Դ
Gold