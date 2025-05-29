## ��Ŀ����
One of the farming chores Farmer John dislikes the most is hauling around lots of cow manure. In order to streamline this process, he comes up with an intriguing idea: instead of hauling manure between two points in a cart behind his tractor, why not shoot it through the air with a giant manure slingshot? (indeed, what could possibly go wrong...)
Farmer John's farm is built along a single long straight road, so any location on his farm can be described simply using its position along this road (effectively a point on the number line). FJ builds $N$ slingshots ($1 \leq N \leq 10^5$), where the $i$th slingshot is described by three integers $x_i$, $y_i$, and $t_i$, specifying that this slingshot can shoot manure from position $x_i$ to position $y_i$ in only $t_i$ total units of time.

FJ has $M$ piles of manure to transport ($1 \leq M \leq 10^5$). The $j$th such pile needs to be moved from position $a_j$ to position $b_j$. Hauling manure with the tractor for a distance of $d$ takes $d$ units of time. FJ is hoping to reduce this by allowing up to one use of any slingshot for transporting each pile of manure. Time FJ spends moving his tractor without manure in it does not count.

For each of the $M$ manure piles, please help FJ determine the minimum possible transportation time, given that FJ can use up to one slingshot during the process.

## �����ʽ
The first line of input contains $N$ and $M$. The next $N$ lines each describe a single slingshot in terms of integers $x_i$, $y_i$, and $t_i$ ($0 \leq x_i, y_i, t_i \leq 10^9$). The final $M$ lines describe piles of manure that need to be moved, in terms of integers $a_j$ and $b_j$.

## �����ʽ
Print $M$ lines of output, one for each manure pile, indicating the minimum time needed to transport it.

## ��Ŀ����
### ��Ŀ����

Farmer John �ϲ����ũ��֮һ���ǵ�������ţ�ࡣΪ�˼���һ���̣��������һ����Ȥ�����⣺������������������ϳ�����ţ�࣬Ϊʲô��ͨ��һ���޴��ţ�൯�������䵽�����أ���ȷʵ�����ܻ��ʲô�����ء�����

Farmer John ��ũ������һ����ֱ�ĳ�·�ϣ����ũ���ϵ��κ�λ�ö����Լ򵥵�����������·�ϵ�λ����������ʵ���Ͼ��������ϵ�һ���㣩��FJ ������ $N$ ��������$1 \leq N \leq 10^5$�������е� $i$ ���������������� $x_i$��$y_i$ �� $t_i$ ��������ʾ����������Խ�ţ���λ�� $x_i$ �䵽λ�� $y_i$������ $t_i$ ����λʱ�䡣

FJ �� $M$ ��ţ����Ҫ���ˣ�$1 \leq M \leq 10^5$������ $j$ ��ţ����Ҫ��λ�� $a_j$ ���˵�λ�� $b_j$��������������ţ�࣬ÿ�ƶ����� $d$ ��Ҫ $d$ ����λʱ�䡣FJ ϣ��ͨ������ÿ��ţ�����ʹ��һ�ε��������ٰ���ʱ�䡣FJ ��û��ţ���������ƶ���������ʱ�䲻�������ʱ�䡣

����ÿ��ţ�࣬����� FJ ȷ�������ʹ��һ�ε���������£��������������ʱ�䡣

### �����ʽ

����ĵ�һ�а��� $N$ �� $M$���������� $N$ ��ÿ������һ�������������������� $x_i$��$y_i$ �� $t_i$��$0 \leq x_i, y_i, t_i \leq 10^9$�������� $M$ ��������Ҫ���˵�ţ��ѣ�ÿ�а����������� $a_j$ �� $b_j$��

### �����ʽ

��� $M$ �У�ÿ�ж�Ӧһ��ţ�࣬��ʾ�������������ʱ�䡣

### ��ʾ

�������һ��ţ����Ҫ��λ�� $1$ ���˵�λ�� $12$�������ʹ�õ������⽫���� $11$ ����λʱ�䡣Ȼ����ʹ�õ�һ������������ $1$ ����λʱ�佫ţ���ƶ���λ�� $0$����������㣩��$1$ ����λʱ�佫ţ���䵽λ�� $10$���������յ㣩��Ȼ�󻨷� $2$ ����λʱ�佫ţ���ƶ���λ�� $12$���ڶ���ţ����ò�ʹ�õ������ˣ���������ţ��Ӧʹ�õڶ����������ˡ�

��Ŀ��Դ��Brian Dean

```input1
2 3
0 10 1
13 8 2
1 12
5 2
20 7
```

```output1
4
3
10
```

## ��ʾ
Here, the first pile of manure needs to move from position 1 to position 12. Without using an slingshot, this would take 11 units of time. However, using the first slingshot, it takes 1 unit of time to move to position 0 (the slingshot source), 1 unit of time to fling the manure through the air to land at position 10 (the slingshot destination), and then 2 units of time to move the manure to position 12. The second pile of manure is best moved without any slingshot, and the third pile of manure should be moved using the second slingshot.

Problem credits: Brian Dean

