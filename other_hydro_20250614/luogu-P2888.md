## ��Ŀ����
Farmer John wants the cows to prepare for the county jumping competition, so Bessie and the gang are practicing jumping over hurdles. They are getting tired, though, so they want to be able to use as little energy as possible to jump over the hurdles.

Obviously, it is not very difficult for a cow to jump over several very short hurdles, but one tall hurdle can be very stressful. Thus, the cows are only concerned about the height of the tallest hurdle they have to jump over.

The cows' practice room has $N$ stations, conveniently labeled $1,\dots,N$. A set of $M$ one-way paths connects pairs of stations; the paths are also conveniently labeled $1,\dots,M$. Path $i$ travels from station $S_i$ to station $E_i$ and contains exactly one hurdle of height $H_i$. Cows must jump hurdles in any path they traverse.

The cows have $T$ tasks to complete. Task $i$ comprises two distinct numbers, $A_i$ and $B_i$, which connote that a cow has to travel from station $A_i$ to station $B_i$ (by traversing over one or more paths over some route). The cows want to take a path the minimizes the height of the tallest hurdle they jump over when traveling from $A_i$ to $B_i$ . Your job is to write a program that determines the path whose tallest hurdle is smallest and report that height.


Farmer John ����������ţ׼��������Ծ������Bessie �����Ļ����������ϰ���������Ǻ��ۣ������������������ٵ������������� ��Ȼ������һͷ��ţ�������������Ǻ����׵ģ����Ǹ���ȴ���ѡ����ǣ���ţ�����ǹ���·������ߵ����ĸ߶ȡ� 

��ţ��ѵ�������� $N$ ��վ̨���ֱ���Ϊ $1,\dots,N$������վ̨֮���� $M$ ������·������ $i$ ��·���Ǵ�վ̨ $S_i$ ��ʼ����վ̨ $E_i$��������ߵ����ĸ߶�Ϊ $H_i$����������ܣ���ţ�Ƕ�Ҫ������ 

��ţ���� $T$ ��ѵ������Ҫ��ɡ��� $i$ ����������������� $A_i$ �� $B_i$����ʾ��ţ�����վ̨ $A_i$ �ܵ�վ̨ $B_i$������·�����վ̨����ţ������һ��·����վ̨ $A_i$ ��վ̨ $B_i$��ʹ·������ߵ����ĸ߶���С�� ����������дһ�����򣬼����·������ߵ����ĸ߶ȵ���Сֵ��


## �����ʽ
\* Line $1$: Three space-separated integers: $N$, $M$, and $T$

\* Lines $2,\dots,M+1$: Line $i+1$ contains three space-separated integers: $S_i$ , $E_i$ , and $H_i$

\* Lines $M+2,\dots,M+T+1$: Line $i+M+1$ contains two space-separated integers that describe task $i$: $A_i$ and $B_i$


��һ�У������ո���������� $N, M, T$��

������ $M$ �У��� $i$ �а��������ո���������� $S_i, E_i, H_i$��

������ $T$ �У��� $i$ �а��������ո��������������ʾ���� $i$ ����ʼվ̨��Ŀ��վ̨ $A_i, B_i$��


## �����ʽ
\* Lines $1,\dots,T$: Line $i$ contains the result for task $i$ and tells the smallest possible maximum height necessary to travel between the stations. Output `-1` if it is impossible to travel between the two stations.

$T$ �У��� $i$ ��Ϊһ����������ʾ���� $i$ ·������ߵ����ĸ߶ȵ���Сֵ������޷������� `-1`��

```input1
5 6 3
1 2 12
3 2 8
1 3 5
2 5 3
3 4 4
2 4 8
3 4
1 2
5 1

```

```output1
4
8
-1

```

## ��ʾ
���� $100\%$ �����ݣ�$1 \le N \le 300$��$1 \le M \le 2.5 \times 10^4$��$1 \le H_i \le 1 \times 10^6$��$1 \le T \le 4 \times 10^4$��$1 \le A_i,B_i \le N$��

��л @gaozhiyong @_Cppsteve_ �ṩ����


