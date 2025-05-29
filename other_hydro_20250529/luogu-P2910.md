## ��Ŀ����
Farmer John is on a boat seeking fabled treasure on one of the N (1 <= N <= 100) islands conveniently labeled 1..N in the Cowribbean Sea.

The treasure map tells him that he must travel through a certain sequence A\_1, A\_2, ..., A\_M of M (2 <= M <= 10,000) islands, starting on island 1 and ending on island N before the treasure will appear to him. He can visit these and other islands out of order and even more than once, but his trip must include the A\_i sequence in the order specified by the map.

FJ wants to avoid pirates and knows the pirate-danger rating (0 <= danger <= 100,000) between each pair of islands. The total danger rating of his mission is the sum of the danger ratings of all the paths he traverses.

Help Farmer John find the least dangerous route to the treasure that satisfies the treasure map's requirement.


## �����ʽ
\* Line 1: Two space-separated integers: N and M

\* Lines 2..M+1: Line i+1 describes the i\_th island FJ must visit with a single integer: A\_i

\* Lines M+2..N+M+1: Line i+M+1 contains N space-separated integers that are the respective danger rating of the path between island i and islands 1, 2, ..., and N, respectively. The ith integer is always zero.


## �����ʽ
\* Line 1: The minimum danger that Farmer John can encounter while obtaining the treasure.


## ��Ŀ����
ũ��Լ������ʻһ��Сͧ��ţ�ձȺ��Ϻ��У�

������ $N(1\leq N\leq 100)$ �����죬�� $1$ �� $N$ ��ţ�Լ���� $1$ ��С����������󵽴� $N$ ��С����

һ�Ųر�ͼ��˵���������·���Ͼ�����С�����γ�����  $A_1,A_2,\dots ,A_M(2\leq M\leq 10000)$ ���������У���һ�����ڣ����������վ����ҵ����ϵı��أ� ���ǣ�����ţ�ձȺ��к�����û��Լ��֪��������������֮��ĺ����Ϻ�����û�ĸ��ʣ�����һ��Σ��ָ�� $D_{i,j}(0\leq D_{i,j}\leq 100000)$ ����������ϣ������Ѱ��������ĺ���Σ��ָ��֮����С����ô�����ҵ����ص�ǰ���£������С��Σ��ָ���Ƕ����أ�

���������ʽ

�����ʽ��

��һ�У������ÿո������������ $N$ �� $M$��

�ڶ����� $M+1$ �У��� $i+1$ ����һ������ $A_i$ ��ʾ FJ ���뾭���ĵ� $i$ ������

�� $M+2$ ���� $N+M+1$ �У��� $i+M+1$ �а��� $N$ ���ÿո�����ķǸ������ֱ��ʾ $i$ ��С������ $1\dots N$ ��С���ĺ��߸��Ե�Σ��ָ������֤�� $i$ ������ $0$��

�����ʽ
��һ�У�FJ ���ҵ����ص�ǰ���¾����ĺ��ߵ�Σ��ָ��֮�͵���Сֵ��

˵��
�������������������죬�ر�ͼҪ�� FJ ��˳�򾭹��ĸ����죺$1$ �ŵ��졢$2$ �ŵ��졢�ص� $1$ �ŵ��졢��� $3$ �ŵ��졣ÿ�����ߵ�Σ��ָ��Ҳ�����ˣ���·$(1,2),(2,3),(3,1)$ �����ǵķ���·����Σ��ָ���ֱ��� $5,2,1$��

FJ ����ͨ�����ξ��� $1,3,2,3,1,3$ �ŵ����� $7$ ����С��Σ��ָ����ñ��ء�������·��������ţ��ͼ��Ҫ�� $(1,2,1,3)$�����Ǳܿ��� $1$ �ź� $2$ �ŵ���֮��ĺ��ߣ���Ϊ����Σ��ָ��̫���ˡ�

ע�⣺���������� $a$ �� $b$ ��Σ��ָ����һ������ $b$ �� $a$ ��Σ��ָ����

Translated by @LJC00125 

```input1
3 4 
1 
2 
1 
3 
0 5 1 
5 0 2 
1 2 0 

```

```output1
7 

```

## ��ʾ
There are 3 islands and the treasure map requires Farmer John to visit a sequence of 4 islands in order: island 1, island 2, island 1 again, and finally island 3. The danger ratings of the paths are given: the paths (1, 2); (2, 3); (3, 1) and the reverse paths have danger ratings of 5, 2, and 1, respectively.


He can get the treasure with a total danger of 7 by traveling in the sequence of islands 1, 3, 2, 3, 1, and 3. The cow map's requirement (1, 2, 1, and 3) is satisfied by this route. We avoid the path between islands 1 and 2 because it has a large danger rating.

���������ʽ


�����ʽ��


��һ�У������ÿո������������N��M


�ڶ�����M+1�У���i+1����һ������Ai��ʾFJ���뾭���ĵ�i������


��M+2����N+M+1�У���i+M+1�а���N���ÿո�����ķǸ������ֱ��ʾi��С������1...N��С���ĺ��߸��Ե�Σ��ָ������֤��i������0��

�����ʽ


��һ�У�FJ���ҵ����ص�ǰ���¾����ĺ��ߵ�Σ��ָ��֮�͵���Сֵ��

˵��

�������������������죬�ر�ͼҪ��FJ��˳�򾭹��ĸ����죺1�ŵ��졢2�ŵ��졢�ص�1�ŵ��졢���3�ŵ��졣ÿ�����ߵ�Σ��ָ��Ҳ�����ˣ���·(1��2)��(2��3)��(3��1)�����ǵķ���·����Σ��ָ���ֱ���5��2��1��


FJ����ͨ�����ξ���1��3��2��3��1��3�ŵ�����7����С��Σ��ָ����ñ��ء�������·��������ţ��ͼ��Ҫ��1��2��1��3�������Ǳܿ���1�ź�2�ŵ���֮��ĺ��ߣ���Ϊ����Σ��ָ��̫���ˡ�


ע�⣺����������a��b��Σ��ָ����һ������b��a��Σ��ָ����


