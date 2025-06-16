## ��Ŀ����
The cows have taken to racing each other around the farm but they get very dizzy when running in circles, and everyone knows that dizzy cows don't produce any milk. Farmer John wants to convert all of the two-way cow paths in the farm to one-way paths in order to eliminate any 'cycles' and prevent the cows from getting dizzy.  A 'cycle' enables a cow to traverse one or more cow paths and arrive back at her starting point, thus completing a loop or circle.

The farm comprises N pastures (1 <= N <= 100,000) conveniently numbered 1..N. M1 (1 <= M1 <= 100,000) one-way cow paths and M2 two-way cow paths (1 <= M2 <= 100,000) connect the pastures. No path directly connects a pasture to itself, although multiple paths might connect two different pastures. A cow may or may not be able to travel between any two given pastures by following a sequence of cow paths.

Your job is to assign a direction to the two-way cow paths such that the entire farm (ultimately with only one-way paths) has no cycles. That is, there should be no sequence of one-way cow paths which leads back to its starting position. The existing one-way cow paths do not form a cycle and should be left as they are.

One-way cow paths run from pasture A\_i (1 <= A\_i <= N) to pasture B\_i (1 <= B\_i <= N). Two-way cow paths connect pastures X\_i (1 <= X\_i <= N) and Y\_i (1 <= Y\_i <= N).

Consider this example:

```cpp
1-->2 
|  /| 
| / | 
|/  | 
3<--4 
```
The cow paths between pastures 1 and 3, 2 and 3, and 2 and 4 are two-way paths. One-way paths connect 1 to 2 and also 4 to 3. One valid way to convert the two-way paths into one-way paths in such a way that there are no cycles would be to direct them from 1 to 3, from 2 to 3, and from 3 to 4:

```cpp
1-->2 
|  /| 
| / | 
vL  v 
3<--4 
```


## �����ʽ
��һ���������� $n,m_1,m_2$���ֱ��ʾ����������ߵ�����������ߵ�������

�ڶ��������� $m_1$ �У�ÿ�� $2$ ������ $a,b$����ʾ $a$ �� $b$ ��һ������ߡ�

���������� $m_2$ �У�ÿ�� $2$ ������ $a,b$����ʾ $a$ �� $b$ �м���һ������ߡ�


## �����ʽ
����ÿ������ߣ�����Ҫ������˳������㶨��Ľ����Ҳ������������ $a\ b$���Ǳ�ʾ�㽫 $a$ �� $b$ �м������߶���Ϊ $a \to b$��

ע�⣬Ҳ����ںܶ���еĽ⡣��ֻҪ�����������һ���ͺá�


## ��Ŀ����
��ţ�Ƿ��֣���ũ�����������Ǻ���Ȥ��һ����.��������һ����ũ�����治�ϵ�תȦ���� ����ͷ��Ŀѣ.������֪��ѣ�ε���ţ���޷����̵�.���ǣ�ũ��Լ����Ҫ����ũ�������˫ ���·ȫ����Ϊ�����·��ʹ������ũ������һ��Ȧ��û�У��Ա���������ţ�Ǳ������ͷת ��.�����ţ���Ծ�����������·�ص���㣬��ô��Щ��·�ͳ�Ϊһ��Ȧ.

ũ���� $n\ (1 < n < 100000)$ Ƭ�ݵأ����Ϊ $1$ �� $n$����Щ�ݵ��� $m_1$ ������ ��·�� $m_2$ ��˫���·��������.�κ�һ����·�������һƬ�ݵغ���Ƭ�ݵر�����������.���ǣ�������Ƭ�ݵ�֮�䶼�����ж�����·����.����֤������Ƭ�ݵ�֮�䶼��· ��������

��������Ǹ����е�˫���·�趨һ������ʹ������ũ��(ֻʣ�µ����·)���һ��Ȧ��û�С�Ҳ����˵��������һ�������·���е��յ������غϡ����ݱ�֤һ��ʼ���еĵ����·�У�һ��Ȧ��û�С�����һ��ʼ���еĵ����·���ܸı䡣

�����·������ǲݵ� $A_i$���յ��ǲݵ� $B_i$��˫���·���Ӳݵ� $X_i,Y_i$��


```input1
4 2 3
1 2
4 3
1 3
4 2
3 2

```

```output1
1 3
4 2
2 3
```

