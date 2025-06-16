## ��Ŀ����
Figuring that they cannot do worse than the humans have, Farmer John's cows have decided to start an airline. Being cows, they decide to cater to the heretofore-untapped market of cows as passengers. They plan to serve the cows who live along the western coast of Lake Michigan. Each morning, they will fly from the northern-most point of the coast southward towards Chicowgo, making many stops along the way. Each evening, they will fly back north to the northernmost point. They need your help to decide which passengers to carry each day. Each of $n \ (1 \le  n \le  10^4)$ farms numbered $1\dots n$ along the coast contains an airport (Farm $1$ is northern-most;farm $n$ is southern-most). On this day,$k \ (1 \le  k \le  5\times 10^4)$ groups of cows wish to travel. Each group of cows wants to fly from a particular farm to another particular farm. The airline, if it wishes, is allowed to stop and pick up only part of a group. Cows that start a flight, however, must stay on the plane until they reach their destination. Given the capacity $c \ (1 \le  c \le  100)$ of the airplane and the groups of cows that want to travel, determine the maximum number of cows that the airline can fly to their destination.

Ϊ�˱�ʾ����������࣬ũ������ţ�Ǿ�������һ�Һ��չ�˾�����Ǽƻ�ÿ���糿������Ъ������������˷������϶ˣ����ϴ����϶˷�����ˡ�����;�У����չ�˾���԰��ŷɻ�ͣ��ĳЩ������������Ҫ�����������ÿ��Я����Щ�ÿ͡����ź������� $n$ ���ɱ����ϱ��Ϊ $1$ �� $n$ ��ũ����ÿ��ũ������һ�����������죬�� $k$ Ⱥţ��Ҫ�����ɻ����С�ÿһȺţ��Ҫ��һ��ũ��������һ��ũ�������������ĳЩũ��ͣ�´��ϲ��ֻ�ȫ���ţ����ţ�ǵǻ����һֱͣ��ֱ���ﵽĿ�ĵ��ṩ����ɻ������� $c$��ͬʱ�ṩ������Ҫ���е���ţ����Ϣ������������һ��ĺ�������ܹ����㼸ֻ��ţ��Ը����

## �����ʽ
* Line $1$: Three space-separated integers: $k,n$, and $c$.
* Lines $2\dots k+1$: Each line contains three space-separated integers $s,e$, and $m$ that specify a group of cows that wishes to travel. The $m \ (1 \le  m \le  c)$ cows are currently at farm $s$ and want to travel to farm $e \ (s \neq e)$.
* ��һ�У�$3$ ���ÿո���������� $k$��$n$ �� $c$��
* �ڶ��� $k+1$ �У�ÿһ���� $3$ ���ÿո���������� $s$��$e$��$m$�� ��ʾ�� $m$ ֻ��ţ���ũ�� $s$ �˷ɻ���ũ�� $e$��
## �����ʽ
* Line $1$: The maximum number of cows that can be flown to their destination. This is the sum of the number of cows flown to their destination on the flight southward in the morning plus the number of cows flown to their destination on the flight northward in the evening.
* ����������е���ţ���������ֵ��

```input1
4 8 3
1 3 2
2 8 3
4 7 1
8 3 2
```

```output1
6
```
## ����˵��

INPUT DETAILS:  
Four groups of cows, eight farms, and three seats on the plane.

$3$ Ⱥ��Ҫ���е���ţ��$8$ ��ũ�����ɻ����� $3$ ����λ���糿���ɻ��� $2$ ֻţ�� $1$ ���� $3$��$1$ ֻţ�� $2$ ���� $8$��$1$ ֻţ�� $4$ ���� $7$�����ϣ������ $2$ ֻţ�� $8$ ���� $3$��
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \le  n \le  10^4$��$1 \leq k \leq 5\times 10^4$��$1 \leq m \leq c \leq 100$��
## ��Ŀ��Դ
Gold