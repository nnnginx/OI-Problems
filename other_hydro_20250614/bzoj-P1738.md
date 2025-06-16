## ��Ŀ����
FJ's cows really hate getting wet so much that the mere thought of getting caught in the rain makes them shake in their hooves. They have decided to put a rain siren on the farm to let them know when rain is approaching. They intend to create a rain evacuation plan so that all the cows can get to shelter before the rain begins. Weather forecasting is not always correct, though. In order to minimize false alarms, they want to sound the siren as late as possible while still giving enough time for all the cows to get to some shelter. The farm has $f \ (1 \le  f \le  200)$ fields on which the cows graze. A set of $p \ (1 \le  p \le  1500)$ paths connects them. The paths are wide, so that any number of cows can traverse a path in either direction. Some of the farm's fields have rain shelters under which the cows can shield themselves. These shelters are of limited size, so a single shelter might not be able to hold all the cows. Fields are small compared to the paths and require no time for cows to traverse. Compute the minimum amount of time before rain starts that the siren must be sounded so that every cow can get to some shelter.

Լ����ţ�Ƿǳ��������꣬�ǻ�ʹ����ɪɪ���������Ǵ��㰲װһ�����걨���������Ұ�����һ�����˼ƻ���������Ҫ�������ٵ�������ţ���������ʱ�䡣ţ����ũ���� $f$ ������ϳԲݡ��� $p$ ��˫��·��������Щ��ء�·�ܿ���������ţ����ͨ��������������������һ����������ţ�ǿ���˲��������ؽ����������ϵ�������������ٵ�ʱ�䣬��ÿֻţ���������
## �����ʽ
* Line $1$: Two space-separated integers: $f$ and $p$.
* Lines $2\dots f+1$: Two space-separated integers that describe a field. The first integer (range: $0\dots 10^3$) is the number of cows in that field. The second integer (range: $0\dots 10^3$) is the number of cows the shelter in that field can hold. Line $i+1$ describes field $i$.
* Lines $f+2\dots f+p+1$: Three space-separated integers that describe a path. The first and second integers (both range $1\dots f$) tell the fields connected by the path. The third integer (range: $1\dots 10^9$) is how long any cow takes to traverse it.

* ��һ�У��������� $f$ �� $p$��
* �ڶ��� $f+1$ �У��� $i+1$ ������������������ $i$ ����أ���һ����ʾ����ϵ�ţ�����ڶ�����ʾ����ϵ����������������������� $0$ �� $10^3$ ֮�䡣
* �� $f+2$ �� $f+p+1$ �У�ÿ��������������һ��·���ֱ�������յ㣬��ͨ������·�����ʱ�䣨�� $1$ �� $10^9$ ֮�䣩��
## �����ʽ
* Line $1$: The minimum amount of time required for all cows to get under a shelter, presuming they plan their routes optimally. If it not possible for the all the cows to get under a shelter, output `-1`.

* һ����������ʾ���ٵ�ʱ�䡣����޷�ʹţ��ȫ������������ `-1`��
```input1
3 4
7 2
0 4
2 6
1 2 40
3 2 70
2 3 90
1 3 120
```
```output1
110
```
## ����˵��
$1$ ����� $7$ ֻţ�У�$2$ ֻţֱ�ӽ��� $1$ ��������$4$ ֻţ���� $1$ ��������$1$ ֻ���� $3$ �������������������� $3$ ��������ţ�ǡ����е�ţ������ $110$ ��λʱ���ڵ���Ҫȥ�����
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq f \leq 200$��$1 \leq p \leq 1500$��
## ��Ŀ��Դ
Gold