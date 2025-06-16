## ��Ŀ����
Bessie is trapped in a triangular maze with N rows (1 <= N <= 1,000,000). A three row maze is shown below:

The i'th row of the maze contains 2\*i-1 triangles. Numbering from the left, the triangles are named (i,1), (i,2), and so on.

Bessie can travel to the (often three) triangles which share an edge with her current triangle. For example, if she is at (3, 3), she can travel to (3, 2), (3, 4) and (4, 4). Bessie takes one minute to travel from one triangle to the next.

FJ has learned the Bessie is trapped and knows by tracking her iPhone that she starts her exit trek at triangle (Si,Sj). FJ's love for Bessie knows no bounds so he wants her back in the minimum possible time.

The maze has M (1 <= M <= 10,000) exits found in locations throughout the set of triangles. Any one of these will enable Bessie to escape. Once she enters an exit triangle, she leaves the maze in just one more minute.

Find the minimum time in minutes, T, required for Bessie to exit the maze and report the optimal exit location she uses, (OUTi, OUTj). If more than one location requires only T minutes, output the location with the smallest row. If two optimal rows are the same, output the one with smaller column.

��ϣ������һ�������ε��Թ�֮�С�����Թ��� $N$ �У�$1 \le N \le 1000000$����������ͼ��һ�� $3$ �е��Թ���  �Թ��ĵ� $i$ ���� $2i-1$ �������Σ������ҷֱ���Ϊ $(i, 1)$��$(i, 2)$ �ȵȡ�

��ϣÿ�ο��Դ�һ���������ߵ�����һ��һ������ǰ�����������ڱߵ������Ρ�

����˵�������Ŀǰ���������� $(3, 3)$����ô���������ߵ������� $(3, 2)$��$(3, 4)$ �� $(4, 4)$����ϣÿ����Ҫһ���ӵ�ʱ�����ƶ�����һ�������Ρ�

ũ��Լ�����ֱ�ϣ�����ˣ����������ٱ�ϣ��iPhone�ֻ��������Ĵ�������������֪��ϣĿǰ���������� $(S_i, S_j)$��

��ΪԼ���Ա�ϣ���������޾���ŨŨ���⣬������ϣ����ϣ�ܾ����ܿ�ػص�������ߡ� ���Թ���������֮�У��� $M$��$1 \le M \le 10000$�����ǳ��ڡ����κ�һ�����ڶ������ñ�ϣ�����Թ���һ����ϣ����һ����Ϊ���ڵ������Σ����ö�һ���ӾͿ�����������Թ��� �ҵ�һ�������ñ�ϣ�����Թ���Сʱ�� $T$���������Ӧ�ô���һ�����������Թ���������ڼ�Ϊ $(\text{OUT}_i, \text{OUT}_j)$��

����ж������ͬʱ��Ҫʱ�� $T$������Ǹ��еı��С�ĳ��ڣ������Ȼ�ж�����ڣ�����Ǹ��еı��С�ġ�


## �����ʽ
\* Line 1: Two space-separated integers: N and M

\* Line 2: Two space-separated integers: Si and Sj

\* Lines 3..M+2: Line i+2 contains two space-separated integers that are the triangle location of exit i: Ei and Ej


## �����ʽ
\* Line 1: Two space-separated integers: OUTi and OUTj

\* Line 2: A single integer: T


```input1
4 2 
2 1 
3 5 
4 4 

```

```output1
4 4 
4 

```

