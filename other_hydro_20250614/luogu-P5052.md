## ��Ŀ����
Branimirko is still a passionate player of the world-renowned game Pok��mon Go. Recently,
he decided to organize a competition in catching Pok��mon. It will be held in Ilica street in
Zagreb, and the main sponsor is his friend Slavko. The reward is, of course, candy!

Ilica is, as we all know, the longest street in Zagreb. There are N houses on the same side of
the street, and each house has a house number between 1 and N. The competition begins
at house number K.

Before the competition, Branimirko looked at the map and saw M Pok��mon. Each Pok��mon
is located at its (distinct) house number Ai
, is valued at Bi candy, and can be caught only in
the next Ti seconds, after which it disappears from the map and is impossible to catch.

Branimirko can visit one house number per second. Also, when he catches a Pok��mon, that
Pok��mon disappears from the map.

Since Branimirko really likes candy, he asked for your help.

Help him and determine the maximal amount of candy he can get!

## �����ʽ
The first line of input contains integers N, K (1 �� K �� N �� 1 000) and M (1 �� M �� 100), the
number of houses, the starting house number and the number of Pok��mon.

Each of the following M lines contains integers $A_i$
(1 �� $A_i$ �� N), $B_i$
(1 �� $B_i$ �� 100) and $T_i$
(1 �� $T_i$ ��
2 000) from the task.
In the input data, the Pok��mon will always be in a strictly ascending order by house number $A_i$ .

## �����ʽ
You must output the required maximal amount of candy from the task.


## ��Ŀ����
Branimirko ������������Ϸ Pok��mon Go ��һλ������ҡ��������������֯һ��ץС����ı������������� Zagreb �� Ilica ��־��У���Ҫ���������������� Slavko��������Ȼ���ǹ�!

���Ƕ�֪����Ilica �� Zagreb ��Ľֵ����ڽֵ���ͬһ���� $N$ �����ӣ����Ӵ����ҷֱ������� $1$ �� $N$ �����ƺš�

����ǰ��Branimirko ���˿���ͼ��������һ���� $M$ ֻС���顣ÿ��С���鶼λ���Լ��ĸ�����ͬ�ķ������ $i$ ���������ƺ�Ϊ $A_i$��С�����ֵ $B_i$ ���ǹ�������ֻ���� $T_i$ ���ڱ�ץ��֮�����ͻ�ӵ�ͼ����ʧ��

Branimirko �� $1$ �������ƺ�Ϊ $K$ �ķ��ӡ�������ÿһ���������ƶ������ƺ����ڵķ��ӣ����߲��ƶ���������һ��ʱ�̺�һֻС���鴦����ͬ�ķ���ʱ�����ͻ�ץס��ֻС���飬������Ӧ���ǹ�������ֻС����ʹӵ�ͼ����ʧ�ˡ�

��Ϊ Branimirko ��ĺ�ϲ���ǹ���������������İ�����

��������������Եõ������ǹ���

### �����ʽ

����ĵ�һ�а����������� $N,K$��$1\le K\le N\le 10^3$���� $M$��$1\le M\le 100$������������Ŀ��������ʼ�ķ������ƺź�С�����������

�������� $M$ ��ÿһ�ж������������� $A_i$��$1\le A_i\le N$����$B_i$��$1\le B_i\le 100$���� $T_i$��$1\le T_i\le 2000$���������������У�С����ʼ�հ��շ���� $A_i$ �ϸ����������

### �����ʽ

����ɻ�ȡ������ǹ�������


### ˵��

�ڲ��������У����� $20\%$ �����ݣ����� $M\le 10$��

�������� $20\%$ �����ݣ����� $M\le 20$��

### ���� 1 ����

һ�ֲ����ǣ�Branimirko �����ڵ� $3$ �����ӣ�$5$ ���ǹ�����׽С���飬Ȼ��ֱ��ڵ� $7$ �����ӣ�$10$ ���ǹ����͵� $9$ �����ӣ�$100$ ���ǹ������ܹ� $115$ ���ǹ���

ע�⵽ Branimirko �޷��� $1$ �ŷ�����ץסС���飬��Ϊ���޷���������ʼλ�ã�$5$ �ŷ��ӣ���ʱ�������


```input1
10 5 4
1 30 4
3 5 7
7 10 12
9 100 23
```

```output1
115 
```

```input2
20 8 7
1 35 14
4 57 1
6 32 2
9 94 28
14 78 8
15 8 1
17 55 3

```

```output2
172
```

## ��ʾ
In test cases worth 20% of total points, it will hold M �� 10.

In additional 20% of total points, it will hold M �� 20.

**Clarification of the first test case:**

One strategy is that Branimirko first catches the Pok��mon at house number 3 (5 candy), then,
respectively, house numbers 7 (10 candy) and 9 (100 candy) for a total of 115 candy.

Notice that Branimirko can��t catch the Pok��mon at house number 1, because he can��t reach it in time
from his starting position (house number 5).

