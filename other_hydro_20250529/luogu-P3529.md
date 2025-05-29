## ��Ŀ����
Bartie and his friends compete in the Team Programming Contest.

There are $n$ contestants on each team, and each team has access to $n$ computers.

The contest lasts $t$ minutes, during which the contestants are to solve $m$ programming problems.

Furthermore, penalties are imposed on the teams: solving a problem $s$ minutes since the beginning of the contest amounts to $s$ penal points.

The team that solved the most problems wins the contest, with ties broken in    favour of the team with smaller penalty.

On the contest day Bartie quickly glances over the problem statements and    distributes them among his teammates.

He knows his team so well that he can exactly assess who is able to solve    which problem.

Solving any problem takes any contestant that is able to solve it exactly $r$ minutes of using the computer.

Bartie's team did not fare well in this year's contest.

Bartie is obsessed with the thought that it might be his fault, due to wrong    decisions regarding the distribution of problems.

He asks you to write a program that, given what Bartie knew at the beginning    of the contest, determines the best possible result of Bytie's team, together    with the assignment of problems to team members that attains the result.


## �����ʽ
Five integers $n$, $m$, $r$, $t$, and $k$ ($1\le n,m\le 500$, $1\le r,t\le 1\ 000\ 000$) are given in the first line of the standard input, separated by single spaces.

These denote, respectively:

the number of contestants on a team, the number of problems, the time it      takes a contestant to solve a problem, the duration of the contest,and the number of contestant-problem pairs given on the input.

Each of the following $k$ lines holds two integers $a$ and $b$($1\le a\le n$,$1\le b\le m$), separated by a single space, denoting that the contestant $a$ is able to solve the problem $b$.Each such pair appears at most once in the input.

In tests worth at least 30% of the points it additionally holds that $n,m\le 100$.


## �����ʽ
In the first line of the standard output the best possible result of Bytie's      team should be printed as two numbers separated by a single space:

the number of solved problems $z$ and the total penal points.

An exemplary assignment of problems that attains this result should be given in the following $z$ lines.

Each of those should hold three integers $a$, $b$ and $c$ ($1\le a\le n$,$1\le b\le m$, $0\le c\le t-r$),separated by single spaces, signifying that the contestant $a$ should start solving the problem $b$ at time $c$(the contest starts at time $0$).No contestant should be assigned a problem that they cannot solve. If more that one optimal assignment exists, your program can output any of them.


## ��Ŀ����
### ��Ŀ����
**���� POI 2011 Round 3. Day 2. C��[Programming Contest](https://szkopul.edu.pl/problemset/problem/VwDLJhYqi1z_sZrb2NyfvQ5e/site/?key=statement)��**

Bartie �����������Ƕ��ڴ����������ƾ�����ÿ������ $n$ ����Ա��ÿ���ӿ����� $n$ ̨���ԡ��������� $t$ ���ӣ�������ѡ����Ҫ��� $m$ �����������Ŀ�����⣬�����ᰴ���¹���Ƿ�ʱ��������ʼ $s$ ����ͨ����һ���⣬��ʱ�� $s$ �֡�������Ŀ���Ķ����ʤ�����������Ŀ��ͬ����ʱ���ٵĶ����ʤ��

��һ�α����У�Bartie Ѹ�������ȫ����Ŀ���Ұ���Ŀ������˶��ѡ���ʮ���˽���ѣ������԰���Ŀ������ܽ���������ˡ�����ÿ��ѡ�֣����һ�����ʱ�䶼ǡ���� $r$ ���ӡ�

Bartie �Ķ����ڽ���ı����б��ֲ��ѡ�Bartie ȷ�������������⣬����������������ʧ����ɵġ���������д�����򣬸��� Bartie �ڱ���ǰ֪������Ϣ������� Bartie �Ķ�����ܵ���óɼ��ͷ�����Ŀ�ķ�ʽ��

### �����ʽ

��һ��������� $n,m,r,t,k$���ֱ��ʾһ�����еĶ�Ա������Ŀ������Ա���һ�������ʱ��������ʱ�䳤�ȺͶ�Ա-��Ŀ������

������ $k$ �У�ÿ�������� $a,b$����ʾ��Ա $a$ ���Խ������ $b$��ÿһ���������������������һ�Ρ�

### �����ʽ

��һ�����������������һ���ո�������ֱ��ʾ�������Ŀ���� $z$ �������ܷ�ʱ��

������ $z$ �У�ÿ������������� $a,b,c\ (1 \le a \le n , 1 \le b \le m , 0 \le c \le t-r)$����ʾ��Ա $a$ ��ʱ�� $c$ ʱ��ʼ�����Ŀ $b$��������ʼ��ʱ�� $0$�����㲻�ܰ�һ�������������������ˡ�����ж��ַ��䷽�����������һ����ɡ�

### ���ݷ�Χ

����ȫ�����ݣ�$ 1 \le n, m \le 500 , 1 \le r, t \le 1000000, 1 \le a \le n , 1 \le b \le m $

���� $30\%$ �ķ�����$n,m\le 100$��

���������� [LibreOJ](https://loj.ac/p/2171)��

```input1
2 4 3 15 4
1 1
2 3
1 4
1 3
```

```output1
3 12
1 4 0
2 3 0
1 1 3
```

