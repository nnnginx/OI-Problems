## ��Ŀ����
Over the years, FJ has made a huge number of farmer friends all around the world. Since he hasn't visited'Farmer Ted'from England and'Boer Harms'from Holland for a while, he'd like to visit them. He knows the longitude of the farm where each of his worldwide friends resides. This longitude is an angle (an integer in the range $0\dots 359$) describing the farm's location on the Earth, which we will consider to be a circle instead of the more complex and traditional spherical representation. Except for the obvious discontinuity, longitudes increase when traveling clockwise on this circle. FJ plans to travel by airplane to visit his $n \ (1 \le  n \le  5\times 10^3)$ friends (whose farms are uniquely numbered $1\dots n$). He knows the schedules for $m \ (1 \le  m \le  2.5\times 10^4)$ bidirectional flights connecting the different farms. Airplanes always travel shortest paths on the Earth's surface (i. e., on the shortest arc of a circle). There will always be a unique shortest path between two farms that are directly connected. No pair of antipodal farms (exactly opposite each other on the circle) is ever directly connected. Each airplane flight can be described as traveling in clockwise or counterclockwise direction around the Earth's surface. For example, a flight from longitude $30$ to longitude $35$ would be clockwise, as would be a flight from longitude $350$ to longitude $10$. However, a flight from longitude $350$ to longitude $200$ follows a shortest path counterclockwise around the circle. FJ would find it very cool if he could make a trip around the world, visiting some of his friends along the way. He'd like to know if this is possible and if so, what is the minimum number of flights he can take to do so. He wants to start and finish his journey at the location of his best friend (the one listed first in the input below). In order to make sure he actually circles the Earth, he wants to ensure that the clockwise distance he travels is different from the counterclockwise distance he travels.

��Щ�꣬ũ��Լ���ڹ����Ͻ���һ������ũ�������ѡ���������һ��ʱ��û��ȥ����Ӣ����ũ��̩�ºͺ�����ũ�򲨶�����������ȥ�������ǣ���֪��ÿ�����ѵ�ũ���ľ��ȡ����ȣ��� $0$ �� $359$����һ�ֽǶ�����ũ���ڵ�����λ�õķ��������ǰѵ��򿴳�һ��Բ��������������֪�ģ������ڵ���������˳ʱ�뷽��������ũ��Լ������˷ɻ�ȥ�������� $n$ �����ѣ��� $1$ �� $n$ ����ʾ������֪������Щũ��֮���� $m$ ��˫��ĺ��ߣ���Ȼ�ɻ��������ŵ�������̵�·�����еģ�����Բ�ϵ���̻�����������ũ��֮��ĺ���һ������̵ģ�Ҳ����˵���������ũ����ֱ�����ˣ���ô����֮��һ�������ں��ߡ������κ�һ�κ��ж����Ա�������˳ʱ�������ʱ��ġ�����˵������ $30$ ������ $35$ ��˳ʱ��ģ����� $350$ ������ $10$ Ҳ��˳ʱ��ģ������� $350$ ������ $200$ ����ʱ��ġ�ũ��Լ��Ϊ��ˣ�ᣬ����Ҫ�����������ѵ�ũ�������������У�����֪�����Ƿ���ܣ������������Ҫ�˼��ηɻ�������������õ����ѣ�Ҳ�����б��еĵ�һ������ũ���Ͽ�ʼ�����������С�Ϊ�˱�֤����һ�λ����У��ص��յ�ʱ��˳ʱ�뾭����·�̲��ܵ�����ʱ�뾭����·�̡�
## �����ʽ
* Line $1$: Two space-separated integers: $n$ and $m$.
* Lines $2\dots n+1$: Line $i+1$ contains one integer: the longitude of the $i$-th farm. Line $2$ contains the location of the farm of his best friend.
* Lines $n+2\dots n+m+1$: Line $i+n+1$ contains two integers giving the indices of two farms that are connected by a flight.
* ��һ�У������ÿո���������� $n$ �� $m$��
* �ڶ��� $n+1$ �У��� $i+1$ ����һ����������ʾ�� $i$ ��ũ���ľ��ȡ��� $2$ ����������õ����ѵĵ�ַ��
* �� $n+2$ ���� $n+m+1$ �У��� $i+n+1$ ����������������ʾ������ũ��֮���к��ߡ�
## �����ʽ
* Line $1$: A single integer specifying the minimum number of flights FJ needs to visit to make a trip around the world.
Every time FJ moves from one farm to another counts as one flight. If it is impossible to make such a trip, output the
integer `-1`.
* һ��������ũ��Լ������Ҫ�˼��ηɻ�������ɻ������С�ÿ��ũ��Լ����һ��ũ��ǰ����һ��ũ��������һ�ηɻ����������������������������� `-1`��

```input1
3 3
0
120
240
1 2
2 3
1 3
```

```output1
3
```
## ����˵��
INPUT DETAILS��  
Farmer John has three friends at longitudes $0,120$, and $240$. There are three flights��$0\leftrightarrow 120,120\leftrightarrow 240$, and $0\leftrightarrow 240$. The journey must start and finish at longitude $0$.

OUTPUT DETAILS��  
FJ must visit all $3$ friends to make a full trip around the world.
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq n \leq 5\times 10^3$��$1 \leq m \leq 2.5\times 10^4$��
## ��Ŀ��Դ
Gold