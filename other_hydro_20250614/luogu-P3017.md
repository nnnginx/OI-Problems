## ��Ŀ����
Bessie has baked a rectangular brownie that can be thought of as an RxC grid (1 <= R <= 500; 1 <= C <= 500) of little brownie squares. The square at row i, column j contains N\_ij (0 <= N\_ij <= 4,000) chocolate chips.

Bessie wants to partition the brownie up into A\*B chunks (1 <= A <= R; 1 <= B <= C): one for each of the A\*B cows. The brownie is cut by first making A-1 horizontal cuts (always along integer

coordinates) to divide the brownie into A strips.  Then cut each strip \*independently\* with B-1 vertical cuts, also on integer

boundaries. The other A\*B-1 cows then each choose a brownie piece, leaving the last chunk for Bessie. Being greedy, they leave Bessie the brownie that has the least number of chocolate chips on it.

Determine the maximum number of chocolate chips Bessie can receive, assuming she cuts the brownies optimally.

As an example, consider a 5 row x 4 column brownie with chips

distributed like this:
```
1 2 2 1
3 1 1 1
2 0 1 3
1 1 1 1
1 1 1 1
```

Bessie must partition the brownie into 4 horizontal strips, each with two pieces. Bessie can cut the brownie like this:

```
1 2 | 2 1
---------
3 | 1 1 1
---------
2 0 1 | 3
---------
1 1 | 1 1
1 1 | 1 1
```

Thus, when the other greedy cows take their brownie piece, Bessie still gets 3 chocolate chips.

## �����ʽ
\* Line 1: Four space-separated integers: R, C, A, and B

\* Lines 2..R+1: Line i+1 contains C space-separated integers: N\_i1, ..., N\_iC


## �����ʽ
\* Line 1: A single integer: the maximum number of chocolate chips that Bessie guarantee on her brownie


## ��Ŀ����
Bessie �決��һ���ɿ������⡣��鵰������ $R\times C(1\leq R,C\leq 500)$ ��С���ɿ���������ɵġ��� $i$ �У��� $j$ �еĵ����� $N_{i,j}(N_{i,j}\leq 4000)$ ���ɿ�����м��

Bessie ��ѵ���ֳ� $A\times B(1\leq A\leq R,1\leq B\leq C)$ �飬�� $A\times B$ ֻ��ţ��������ˮƽ���� $A-1$ ����ֻ���������������У����ѵ��⻮�ֳ� $A$ �顣Ȼ���ٰ�ʣ������ÿһ��������� $B-1$ ����Ҳֻ���������������С����� $A\times B-1$ ֻ��ţ��ÿ��ѡһ�飬����һ��� Bessie������̰�ģ�����ֻ������ Bessie �ɿ�����м���ٵ��ǿ顣��� Bessie ��������»��ö����ɿ�����м��

���磬����һ�� $5\times4$ �ĵ��⣬�������м�ֲ�����ͼ��ʾ��
```
1 2 2 1
3 1 1 1
2 0 1 3
1 1 1 1
1 1 1 1
```
Bessie����ѵ����г�4����ÿ���ֳ�2�顣Bessie���������е���:
```
1 2 | 2 1
---------
3 | 1 1 1
---------
2 0 1 | 3
---------
1 1 | 1 1
1 1 | 1 1
```
������Bessie�����ܻ�� $3$ ���ɿ�����м��

```input1
5 4 4 2 
1 2 2 1 
3 1 1 1 
2 0 1 3 
1 1 1 1 
1 1 1 1 

```

```output1
3 

```

