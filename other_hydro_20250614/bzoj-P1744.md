## ��Ŀ����
Bessie and the rest of Farmer John's cows are taking a trip this winter to go skiing. One day Bessie finds herself at the top left corner of an $r \ (1 \le  r \le  100)$ by $c \ (1 \le  c \le  100)$ grid of elevations $e \ (-25 \le  e \le  25)$. In order to join FJ and the other cows at a discow party, she must get down to the bottom right corner as quickly as she can by travelling only north, south, east, and west. Bessie starts out travelling at a initial speed $v \ (1 \le  v \le  10^6)$. She has discovered a remarkable relationship between her speed and her elevation change. When Bessie moves from a location of height $a$ to an adjacent location of height $b$, her speed is multiplied by the number $2^{a-b}$. The time it takes Bessie to travel from a location to an adjacent location is the reciprocal of her speed when she is at the first location. Find the both smallest amount of time it will take Bessie to join her cow friends and the number of moves required by the path (a move is a transition from one location to another adjacent location).

���������һЩ��ȥ��ѩ�����緢�����Լ�վ��һ�� $r \times c$ �������У������е�ÿһ�鶼��һ���߶�ֵ $e_{i,j}$��Ϊ�˲μӴ�ҵľۻᣬ������Ҫ���쵽�����½ǡ�����ÿһ��ֻ�������������������ϣ�����ǰ��һ���������Գ��ٶ� $v$ ǰ������������һ�������ٶȺ͸߶ȵĹ�ϵ��������Ӹ߶� $a$ �ƶ����߶� $b$�������ٶȾͳ�����һ���� $2^{a-b}$�������ƶ�һ�����ٶ�ȡ��������ǰһ��ʱ���ٶȡ����ҳ������ƶ��������Сʱ�䡣
## �����ʽ
* Line $1$: Three space-separated integers: $v,r$, and $c$, which respectively represent Bessie's initial velocity and the number of rows and columns in the grid.
* Lines $2\dots r+1$: $c$ integers representing the elevation $e$ of the corresponding location on the grid.
* ��һ�У�$3$ ���ÿո���������� $v,r,c$���ֱ��ʾ����ĳ��ٶȺ�����ĳ��ȺͿ�ȡ�
* �ڶ��� $r+1$ �У��Ծ������ʽ��ʾ�������и���ĸ߶ȡ�
## �����ʽ
A single number value, printed to two exactly decimal places: the minimum amount of time that Bessie can take to reach the bottom right corner of the grid.  
���һ��ʵ����**���� $2$ λС��**������ʾ����ﵽĿ�ĵ�������Ҫ��ʱ�䡣
```input1
1 3 3
1 5 3
6 3 5
2 4 3
```
```output1
29.00
```
## ����˵��
��ţ��ʼ�����Ͻǣ��ٶ�Ϊ $1$���������ƶ�����ĸ����ϣ��ٶȻᷢ���仯��  
$3\times 3$ �����������ÿ�����ӵĲ���������һ������ $a$ �� $b$ ʱ���ٶȱ�� $v\times 2^{a-b}$��

OUTPUT DETAILS:  
Bessie's best route is:  
Start at $\ (1,1)$ time $0$ speed $1$.  
East to $\ (1,2)$ time $1$ speed $\dfrac{1}{16}$.  
South to $\ (2,2)$ time $17$ speed $\dfrac{1}{4}$.  
South to $\ (3,2)$ time $21$ speed $\dfrac{1}{8}$.  
East to $\ (3,3)$ time $29$ speed $\dfrac{1}{4}$.  
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq r,c \leq 100$��$-25 \le  e_{i,j} \le  25$��$1 \leq v \leq 10^6$��
## ��Ŀ��Դ
Gold