## ��Ŀ����
BaoBao and DreamGrid are playing the game $\textit{Plants vs. Zombies}$. In the game, DreamGrid grows plants to defend his garden against BaoBao's zombies.

![](https://cdn.luogu.com.cn/upload/image_hosting/9tyl9ix3.png)

$\textit{Plants vs. Zombies(?)} \\
\textit{(Image from pixiv. ID: 21790160; Artist: socha)}$

There are $n$ plants in DreamGrid's garden arranged in a line. From west to east, the plants are numbered from 1 to $n$ and the $i$-th plant lies $i$ meters to the east of DreamGrid's house. The $i$-th plant has a defense value of $d_i$ and a growth speed of $a_i$. Initially, $d_i = 0$ for all $1 \le i \le n$. 

DreamGrid uses a robot to water the plants. The robot is in his house initially. In one step of watering, DreamGrid will choose a direction (east or west) and the robot moves exactly 1 meter along the direction. After moving, if the $i$-th plant is at the robot's position, the robot will water the plant and $a_i$ will be added to $d_i$. Because the water in the robot is limited, at most $m$ steps can be done.

The defense value of the garden is defined as $\min\{d_i | 1 \le i \le n\}$. DreamGrid needs your help to maximize the garden's defense value and win the game.

- Each time the robot MUST move before watering a plant;
- It's OK for the robot to move more than $n$ meters to the east away from the house, or move back into the house, or even move to the west of the house.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($2 \le n \le 10^5$, $0 \le m \le 10^{12}$), indicating the number of plants and the maximum number of steps the robot can take.

The second line contains $n$ integers $a_1, a_2, ... , a_n$ ($1 \le a_i \le 10^5$), where $a_i$ indicates the growth speed of the $i$-th plant.

It's guaranteed that the sum of $n$ in all test cases will not exceed $10^6$.

## �����ʽ
For each test case output one line containing one integer, indicating the maximum defense value of the garden DreamGrid can get.

## ��Ŀ����
���� $n$ ��ֲ��� $m$ �Ĳ������ƣ�ÿ��ֲ����λ�� $1\dots n$ �ϡ����ʼʱ��λ�� $0$��ÿ�ο����ƶ������ڵ�λ���ϡ�

ÿ����������һ���󵽴��λ���� $i$�����ʹ�����λ�õ�ֲ��ĸ߶����� $a_i$���� $d_i$ Ϊ���� $m$ ����λ�� $i$ ��ֲ��߶ȣ����һ�����ŵ��߷�ʹ�� $\min\limits_{1 \le i \le n} d_i$ ���

$2\leq n\leq 10 ^ 5$��$0\leq m\leq 10 ^ {12}$��$1\leq a_i\leq 10 ^ 5$��$\sum n\leq 10 ^ 6$��

```input1
2
4 8
3 2 6 6
3 9
10 10 1
```

```output1
6
4
```

## ��ʾ
In the explanation below, `E` indicates that the robot moves exactly 1 meter to the east from his current position, and `W` indicates that the robot moves exactly 1 meter to the west from his current position.

For the first test case, a candidate direction sequence is $\{E, E, W, E, E, W, E, E\}$, so that we have $d = \{6,6,12,6\}$ after the watering.

For the second test case, a candidate direction sequence is $\{E, E, E, E, W, E, W, E, W\}$, so that we have $d = \{10, 10, 4\}$ after the watering.

