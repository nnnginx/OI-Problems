## ��Ŀ����
Every day, Farmer John walks through his pasture to check on the well-being ofeach of his cows. On his farm he has two breeds of cows, Holsteins and Guernseys. His $H$ Holsteins are conveniently numbered $1 \ldots H$, and his $G$ Guernseys are conveniently numbered $1 \ldots G$($1 \leq H \leq 1000, 1 \leq G \leq 1000$). Each cow is located at a point inthe 2D plane (not necessarily distinct).

Farmer John starts his tour at Holstein 1, and ends at Holstein $H$.  He wantsto visit each cow along the way, and for convenience in maintaining hischecklist of cows visited so far, he wants to visit the Holsteins and Guernseysin the order in which they are numbered. In the sequence of all $H+G$ cows hevisits, the Holsteins numbered $1 \ldots H$ should appear as a (not necessarilycontiguous) subsequence, and likewise for the Guernseys. Otherwise stated, thesequence of all $H+G$ cows should be formed by  interleaving the list ofHolsteins numbered $1 \ldots H$ with the list of Guernseys numbered $1 \ldots G$.

When FJ moves from one cow to another cow traveling a distance of $D$, heexpends $D^2$ energy.  Please help him determine the minimum amount of energyrequired to visit all his cows according to a tour as described above.

## �����ʽ
The first line of input contains $H$ and $G$, separated by a space.

The next $H$ lines contain the $x$ and $y$ coordinates of the $H$ Holsteins, and the next $G$ lines after that contain coordinates of the Guernseys. Each coordinate is an integer in the range $0 \ldots 1000$.


## �����ʽ
Write a single line of output, giving the minimum energy required for FJ's tour of all the cows.


## ��Ŀ����
### ��Ŀ����

ÿ�죬Farmer John ���ᴩ���������������ÿͷ��ţ�Ľ���״��������ũ������������ţ����˹̹ţ�͸���ţ������ $H$ ͷ��˹̹ţ������ر��Ϊ $1 \ldots H$�������� $G$ ͷ����ţ������ر��Ϊ $1 \ldots G$��$1 \leq H \leq 1000, 1 \leq G \leq 1000$����ÿͷ��ţ��λ�ڶ�άƽ���е�һ���㣨��һ����ͬ����

Farmer John �Ӻ�˹̹ţ 1 ��ʼ����Ѳ�ӣ����ں�˹̹ţ $H$ ��������ϣ����;����ÿͷ��ţ������Ϊ�˷���ά�����Ѿ����ʹ�����ţ�嵥����ϣ�����ձ��˳����ʺ�˹̹ţ�͸���ţ���������ʵ����� $H+G$ ͷ��ţ�������У����Ϊ $1 \ldots H$ �ĺ�˹̹ţӦ��Ϊһ������һ�������ģ������г��֣�ͬ���أ����Ϊ $1 \ldots G$ �ĸ���ţҲӦ��ˡ����仰˵������ $H+G$ ͷ��ţ������Ӧͨ�������Ϊ $1 \ldots H$ �ĺ�˹̹ţ�б�����Ϊ $1 \ldots G$ �ĸ���ţ�б������ж��ɡ�

�� Farmer John ��һͷ��ţ�ƶ�����һͷ��ţ���ƶ�����Ϊ $D$ ʱ���������� $D^2$ ���������������ȷ����������Ѳ�ӷ�ʽ����������ţ�������С������

### �����ʽ

����ĵ�һ�а����ÿո�ָ��� $H$ �� $G$��

�������� $H$ �а��� $H$ ͷ��˹̹ţ�� $x$ �� $y$ ���꣬���� $G$ �а�������ţ�����ꡣÿ�����궼�� $0 \ldots 1000$ ��Χ�ڵ�������

### �����ʽ

���һ�У���ʾ Farmer John Ѳ��������ţ�������С������

```input1
3 2
0 0
1 0
2 0
0 3
1 3
```

```output1
20
```

