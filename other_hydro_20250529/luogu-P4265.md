## ��Ŀ����
It's winter on the farm, and that means snow! There are $N$ tiles on the path from the farmhouse to the barn, conveniently numbered $1 \dots N$, and tile $i$ is covered in $f_i$ feet of snow.
Farmer John starts off on tile $1$ and must reach tile $N$ to wake up the cows. Tile $1$ is sheltered by the farmhouse roof, and tile $N$ is sheltered by the barn roof, so neither of these tiles has any snow. But to step on the other tiles, Farmer John needs to wear boots!

In his foul-weather backpack, Farmer John has $B$ pairs of boots, numbered $1 \dots B$. Some pairs are more heavy-duty than others, and some pairs are more agile than others. In particular, pair $i$ lets FJ step in snow at most $s_i$ feet deep, and lets FJ move at most $d_i$ forward in each step.

Unfortunately, the boots are packed in such a way that Farmer John can only access the topmost pair at any given time. So at any time, Farmer John can either put on the topmost pair of boots (discarding his old pair) or discard the topmost pair of boots (making a new pair of boots accessible).

Farmer John can only change boots while standing on a tile. If that tile has $f$ feet of snow, both the boots he takes off AND the boots he puts on must be able to withstand at least $f$ feet of snow. Intermediate pairs of boots which he discards without wearing do not need to satisfy this restriction.

Help Farmer John minimize waste, by determining the minimum number of pairs of boots he needs to discard in order to reach the barn. You may assume that Farmer John is initially not wearing any boots.

## �����ʽ
The first line contains two space-separated integers $N$ and $B$ ($2 \leq N,B \leq 250$).
The second line contains $N$ space-separated integers. The $i$th integer is $f_i$, giving the depth of snow on tile $i$ ($0 \leq f_i \leq 10^9$). It's guaranteed that $f_1 = f_N = 0$.

The next $B$ lines contain two space-separated integers each. The first integer on line $i+2$ is $s_i$, the maximum depth of snow in which pair $i$ can step. The second integer on line $i+2$ is $d_i$, the maximum step size for pair $i$. It's guaranteed that $0 \leq s_i \leq 10^9$ and $1 \leq d_i \leq N-1$.

The boots are described in top-to-bottom order, so pair $1$ is the topmost pair in FJ's backpack, and so forth.

## �����ʽ
The output should consist of a single integer, giving the minimum number of boots Farmer John needs to discard. It's guaranteed that it will be possible for FJ to make it to the barn.

## ��Ŀ����
### ��Ŀ����

ũ���Ķ��쵽�ˣ�����ζ����ѩ�ˣ���ũ�ᵽ�Ȳֵ�·���� $N$ ���ש������ر��Ϊ $1 \dots N$���� $i$ ���ש�ϸ����� $f_i$ Ӣ�ߵ�ѩ��

Farmer John �ӵ� $1$ ���ש���������뵽��� $N$ ���שȥ������ţ���� $1$ ���ש��ũ����ݶ��ڱΣ��� $N$ ���ש���Ȳֵ��ݶ��ڱΣ�����������ש��û��ѩ����Ҫ����������ש�ϣ�Farmer John ��Ҫ��ѥ�ӣ�

�����Ķ������������У�Farmer John �� $B$ ˫ѥ�ӣ����Ϊ $1 \dots B$����Щѥ�ӱ�����ѥ�Ӹ����ã���Щѥ�ӱ�����ѥ�Ӹ���������˵���� $i$ ˫ѥ������ Farmer John ����� $s_i$ Ӣ�����ѩ�����ߣ�����ÿ���������ƶ� $d_i$ ���ש��

���ҵ��ǣ�ѥ�ӵĴ����ʽʹ�� Farmer John ���κ�ʱ��ֻ�ܷ����������һ˫ѥ�ӡ���ˣ�Farmer John ������ʱ�����������һ˫ѥ�ӣ�������ѥ�ӣ������������һ˫ѥ�ӣ�ʹ��һ˫ѥ�ӿɷ��ʣ���

Farmer John ֻ���ڵ�ש�ϸ���ѥ�ӡ�����õ�ש���� $f$ Ӣ�ߵ�ѩ����ô�����µ�ѥ�Ӻʹ��ϵ�ѥ�Ӷ������ܹ��������� $f$ Ӣ�ߵ�ѩ����������δ�������м�ѥ�Ӳ���Ҫ��������ơ�

����� Farmer John ��С���˷ѣ�ȷ��������Ȳ���Ҫ����������ѥ�Ӷ��������� Farmer John ���û�д��κ�ѥ�ӡ�

### �����ʽ

��һ�а��������Կո�ָ������� $N$ �� $B$��$2 \leq N, B \leq 250$����

�ڶ��а��� $N$ ���Կո�ָ����������� $i$ �������� $f_i$����ʾ�� $i$ ���ש�ϵ�ѩ����ȣ�$0 \leq f_i \leq 10^9$������֤ $f_1 = f_N = 0$��

�������� $B$ ��ÿ�а��������Կո�ָ����������� $i+2$ �еĵ�һ�������� $s_i$����ʾ�� $i$ ˫ѥ�ӿ��Գ��ܵ����ѩ��ڶ��������� $d_i$����ʾ�� $i$ ˫ѥ�ӵ���󲽳�����֤ $0 \leq s_i \leq 10^9$ �� $1 \leq d_i \leq N-1$��

ѥ�Ӱ����ϵ��µ�˳����������˵� $1$ ˫ѥ���Ǳ������������һ˫���������ơ�

### �����ʽ

���Ӧ����һ����������ʾ Farmer John ��Ҫ����������ѥ�Ӷ�������֤ Farmer John �ܹ�����Ȳ֡�

### ��ʾ

��Ŀ��Դ��Brian Dean �� Dhruv Rohatgi

```input1
10 4
0 2 8 3 6 7 5 1 4 0
2 3
4 2
3 4
7 1
```

```output1
2

```

## ��ʾ
Problem credits: Brian Dean and Dhruv Rohatgi

