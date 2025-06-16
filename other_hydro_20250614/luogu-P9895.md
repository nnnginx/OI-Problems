## ��Ŀ����
PUBG is a multiplayer online battle royale video game. In the game, up to one hundred players parachute onto an island and scavenge for weapons and equipment to kill others while avoiding getting killed themselves. Airdrop in this game is a key element, as airdrops often carry with them strong weapons or numerous supplies, helping players to survive.

![](https://cdn.luogu.com.cn/upload/image_hosting/qv9hzuoe.png)
textit{Airdrop in the game(?)

Consider the battle field of the game to be a two-dimensional plane. An airdrop has just landed at point $(x_0, y_0)$ (both $x_0$ and $y_0$ are integers), and all the $n$ players on the battle field, where $(x_i, y_i)$ (both $x_i$ and $y_i$ are integers) indicates the initial position of the $i$-th player, start moving towards the airdrop with the following pattern:


- If the position of a living player at the beginning of this time unit is not equal to $(x_0, y_0)$, he will begin his next move.
- + Let's say he is currently at point $(x, y)$. For his next move, he will consider four points $(x, y - 1)$, $(x, y + 1)$, $(x - 1, y)$ and $(x + 1, y)$.
- + He will select one of the four points whose Manhattan distance to the airdrop $(x_0, y_0)$ is the smallest to be the destination of his next move. Recall that the Manhattan distance between two points $(x_a, y_a)$ and $(x_b, y_b)$ is defined as $|x_a - x_b| + |y_a - y_b|$.
- + If two or more points whose Manhattan distance to the airdrop is the same, he will use the following priority rule to break the tie: $(x, y - 1)$ has the highest priority to be selected, $(x, y + 1)$ has the second highest priority, $(x - 1, y)$ has the third highest priority, and $(x + 1, y)$ has the lowest priority.
- + At the end of this time unit, he arrives at his destination.
- If the position of a living player at the beginning of this time unit is equal to $(x_0, y_0)$, he will continue to fatten his backpack with the supplies in the airdrop and stays at $(x_0, y_0)$.


But the battle is tough and it's almost impossible for all the players to arrive at the airdrop safely. If two or more players meet at point $(x', y')$ other than $(x_0, y_0)$, where both $x'$ and $y'$ are integers, they will fight and kill each other and none of them survive.

BaoBao is a big fan of the game and is interested in the number of players successfully arriving at the position of the airdrop, but he doesn't know the value of $x_0$. Given the value of $y_0$ and the initial position of each player, please help BaoBao calculate the minimum and maximum possible number of players successfully arriving at the position of the airdrop for all $x_0 \in \mathbb{Z}$, where $\mathbb{Z}$ is the set of all integers (note that $x_0$ can be positive, zero or negative).


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $y_0$ ($1 \le n \le 10^5$, $1 \le y_0 \le 10^5$), indicating the number of players and the $y$ value of the airdrop.

For the following $n$ lines, the $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 10^5$), indicating the initial position of the $i$-th player.

It's guaranteed that the sum of $n$ in all test cases will not exceed $10^6$, and in each test case no two players share the same initial position.


## �����ʽ
For each test case output one line containing two integers $p_\text{min}$ and $p_\text{max}$ separated by one space. $p_\text{min}$ indicates the minimum possible number of players successfully arriving at the position of the airdrop, while $p_\text{max}$ indicates the maximum possible number.


## ��Ŀ����
### ��Ŀ����
�� $n$ �������һ��ƽ��ֱ������ϵ�д� PUBG. ��ʱһ����Ͷ������ $(x_0, y_0)$ ��.

���ڳ��ϻ�ʣ $n$ �����������. �ӿ�Ͷ��ص�ʱ����, ÿһ��ʱ��ִ�����²��� :

1. �ƶ��׶�

����ÿ����������� :
- ����䲻�� $(x_0, y_0)$ :
  - ���Ͷ������ $x$ ��**��** $y$ �᷽���ƶ� $1$ ����λ����, ʹ���ƶ���λ���� $(x_0, y_0)$ �������پ��뾡����С. 
  - ����һ������Ļ�����, ����ж��ַ���Ҫ����ƶ���ʽ, �������� $y$ ���ƶ�.
- ������� $(x_0, y_0)$, �򲻽��в���.

2. ս���׶�

�ƶ��׶ν�����, ���**�� $(x_0, y_0)$ ��**����һ����ڳ��� $1$ �����, ����һ����������ж�Ϊ�����������Ƴ���Ϸ.

---

����֤��, �����㹻��β�����, �����ԡ�������Ҷ��ᴦ�� $(x_0, y_0)$ λ��.

���� $y_0$, �� $x_0$ ȡ��������ֵʱ, ���ա�������������ֵ����Сֵ.

### ���������ʽ�����ݷ�Χ
���ȸ���һ������ $T$, ��ʾ��������. ����������ÿ������ :

��һ�и������������� $n, y_0$, ������������.

������ $n$ ��, ÿ������������ $x, y$, ��ʾ $n$ ����ҵ�����.

$n$ �����е������ֵ�������� $10^5$, �ұ�֤������������ҳ�ʼ����ͬһλ��. �������Ե�� $\sum n \le 10^6$.

**ע�� : $x_0$ ����ȡ $0$ ��ֵ, �Ҳ�������ֵ������ $10^5$ ������.**

����ÿ������, ���һ�� 2 ���ո�ֿ�������, �ֱ��ʾ���ա�������������ֵ����Сֵ.

Translated by @[Ja50nY0un9](/user/363302).

```input1
3
3 2
1 2
2 1
3 5
3 3
2 1
2 5
4 3
2 3
1 3
4 3
```

```output1
1 3
0 3
2 2
```

## ��ʾ
We now explain the first sample test case.

To obtain the answer of $p_\text{min} = 1$, one should consider $x_0 = 3$. The following table shows the position of each player at the end of each time unit when $x_0 = 3$.

![](https://cdn.luogu.com.cn/upload/image_hosting/itsnfe48.png)

To obtain the answer of $p_\text{max} = 3$, one should consider $x_0 = 2$. The following table shows the position of each player at the end of each time unit when $x_0 = 2$.

![](https://cdn.luogu.com.cn/upload/image_hosting/hvseoyfc.png)

