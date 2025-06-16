## ��Ŀ����
You have been hired by Addictive Coin Machines to help design the next hit in their line of eye-catching, coin-guzzling, just-one-more-try Pachinko machines for casinos around the world.

Playing a Pachinko machine involves launching balls into a rectangular grid filled with pegs, obstacles, and targets. The ball bounces around the grid until it eventually hits one of the targets. The player earns a certain number of points depending on which target is hit.

The grid pattern for the next Pachinko machine has already been designed, but point values for the targets have not been assigned. These must be set so that like all casino machines, the machine is profitable but not too profitable. Thus it is important to figure out the probability of a ball hitting any particular target. That��s your job!

For simplicity, the grid is modeled as a tall rectangle filled with mostly-open spaces (each represented by ��.��), impassable obstacles (each represented by ��X��), and targets (each represented by ��T��).

A ball is launched randomly with uniform probability into one of the mostly-open spaces on the top row of the grid. From that point on, collisions with pegs cause the ball to randomly bounce up, down, left, or right, with various given probabilities. For simplicity, assume these probabilities are the same for every space in the grid. If the ball bounces into an obstacle or attempts to move off the grid, it won��t actually move from its current space. When the ball moves into a target it is removed from play.

You can safely assume that the average number of spaces visited by a ball before hitting a target will not exceed $10^{9}$. It would not make for a very enjoyable game if the ball just bounces forever!

For each target, calculate the probability that it is the one hit by a launched ball.

## �����ʽ
The input consists of a single test case. The first line contains integers $w$ and $h$, which are the width and height of the Pachinko grid ($1 \leq w \leq 20$ and $2 \leq h \leq 10\, 000$). The next line contains four non-negative integers $u$, $d$, $l$, and $r$, which sum to 100 and are the percentage probabilities of the ball bouncing up, down, left, or right from any open space.

Each of the next $h$ lines contains $w$ characters, each of which is ��.��, ��X��, or ��T��. These lines describe the Pachinko grid. The first line, which describes the top row of the grid, contains at least one ��.�� and no ��T��s.

## �����ʽ
Display one line for each ��T�� in the grid, in order from top to bottom, breaking ties left to right. For each target, display the probability that a launched ball will hit it. Give the answer with an absolute error of at most $10^{-6}$.

## ��Ŀ����
**��Ŀ����**

��һ�����Ϊ $w$ �߶�Ϊ $h$ �ķ���ֽ�� $ w \times h$ �ĸ����У���һЩ�ǿյģ���һЩ�Ƕ�����һЩ���ϰ���ӵ�һ�еĿյĸ��������ѡһ������һ���������������ƶ��ĸ��ʱ�Ϊ $p_u : p_d : p_l : p_r$������ $p_u + p_d + p_l + p_r = 100$���������ƶ������ϰ���ĸ����ϡ�����ÿ�������������ö��ĸ��ʡ�$w \le 20, h \le 10000$����֤��һ��û�ж���

**�����ʽ**

��һ������������ʾ $w, h$ ��

�ڶ����ĸ�������ʾ $p_u, p_d, p_l, p_r$ ��

��������һ�� $h$ �� $w$ ���ַ��������� `.` ��ʾ�գ�`X` ��ʾ�ϰ��`T` ��ʾ����

**�����ʽ**

�����У�ÿһ��һ�����������վ�����ϵ��£������ҵ�˳�����ÿ�����Ĵ𰸡����������� $10^{-6}$ ��Ϊ��ȷ��

```input1
3 2
20 20 20 40
X.X
T.T

```

```output1
0.333333333
0.666666667

```

```input2
4 5
12 33 28 27
....
.XX.
....
T..T
XTTX

```

```output2
0.435853889
0.403753221
0.081202502
0.079190387

```

## ��ʾ
Time limit: 5000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2014

