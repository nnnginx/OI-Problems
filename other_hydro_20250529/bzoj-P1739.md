## ��Ŀ����
The cows are going to space! They plan to achieve orbit by building a sort of space elevator:  
a giant tower of blocks. They have $k \ (1 \le k \le 400)$ different types of blocks with which to build the tower. Each block of type $i$ has height $h_i \ (1 \le h_i \le 100)$ and is available in quantity $c_i \ (1 \le c_i \le 10)$. Due to possible damage caused by cosmic rays, no part of a block of type $i$ can exceed a maximum altitude $a_i \ (1 \le a_i \le 4\times 10^4)$. Help the cows build the tallest space elevator possible by stacking blocks on top of each other according to the rules.

ţ��Ҫ��̫��ȥ�ˣ����Ǵ��㽨��һ��̫�յ����������ǽ�������  
�� $k$ �ַ��飬�� $i$ ����һ���ض��ĸ߶� $h_i$��һ���Ĵ��� $c_i$. Ϊ���������ߵ��ƻ����� $i$ �ַ�����κβ��ֲ��ܳ����߶� $a_i$��������Щ����ѳ���ߵ�̫�յ��ݡ�

## �����ʽ
* Line $1$: A single integer, $k$.
* Lines $2 \ldots k+1$: Each line contains three space-separated integers: $h_i,a_i$, and $c_i$. Line $i+1$ describes block type $i$.
* ��һ������һ������ $k$��
* ������ $k$ �У�ÿ�������������� $h_i,a_i,c_i$��
## �����ʽ
* Line $1$: A single integer $h$, the maximum height of a tower that can be built.
* һ����������ʾ���߶ȡ�
```input1
3
7 40 3
5 23 8
2 52 6
```
```output1
48
```
## ����˵��
�ӵײ���ʼ���ȷ� $3$ ������ $2$��֮�� $3$ ������ $1$�������� $6$ ������ $3$�����ܰ� $3$ ������ $1$ �ѵ� $4$ ������ $2$ �ϣ���Ϊ������ߵķ��� $1$ �Ķ����߶ȳ����� $40$��
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq k \leq 400$��$1 \leq h_i \leq 100$��$1 \leq c_i \leq 10$��$1 \leq a_i \leq 4\times 10^4$��
## ��Ŀ��Դ
Gold