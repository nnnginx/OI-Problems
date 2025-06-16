## ��Ŀ����
Farmer John has lost his favorite cow bell, and Bessie the cow has agreed to help him find it!  They both fan out and search the farm along different paths, but stay in contact via radio so they can keep in touch with each-other. Unfortunately, the batteries in their radios are running low, so they want to plan their movements so as to conserve power, by trying to stay always within a short distance apart.

Farmer John starts at location ($f_x, f_y$) and plans to follow a path consisting of  $N$ steps, each of which is either 'N' (north), 'E' (east), 'S' (south), or 'W' west.  Bessie starts at location ($b_x, b_y$) and follows a similar path consisting of $M$ steps.  Both paths may share points in common.  At each time step, Farmer John can either stay put at his current location, or take one step forward along his path, in whichever direction happens to be next (assuming he has not yet reached the final location in his path). Bessie can make a similar choice.  At each time step (excluding the first step where they start at their initial locations), their radios consume energy equal to the square of the distance between them.

Please help FJ and Bessie plan a joint movement strategy  that will minimize the total amount of energy consumed up to and including the final step where both of them first reach the final locations on their respective paths.

## �����ʽ
The first line of input contains $N$ and $M$ ($1 \leq N, M \leq 1000$). The second line contains integers $f_x$ and $f_y$, and the third line contains $b_x$ and $b_y$ ($0 \leq f_x, f_y, b_x, b_y \leq 1000$). The next line contains a string of length $N$ describing FJ's path, and the final line contains a string of length $M$ describing Bessie's path.

It is guranteed that Farmer John and Bessie's coordinates are always in the range ($0 \leq x,y \leq 1000$) throughout their journey. Note that East points in the positive x direction and North points in the positive y direction.

## �����ʽ
Output a single integer specifying the minimum energy FJ and Bessie can use during their travels.

## ��Ŀ����
### ��Ŀ����

FJ ʧȥ������ϲ����ţ�壬�� Bessie �Ѿ�ͬ��������ҵ����������ò�ͬ��·������ũ����ͨ�����ߵ籣����ϵ��

���ҵ��ǣ����ߵ��еĵ�ص������㣬���������跨�����ܱ�������λ�õľ�����С���Խ�ʡ������

FJ ��λ��$(f_x,f_y)$ ��ʼ�����ƻ���ѭ�� $N$ ����ɵ�·��.Bessie ��λ�� $(b_x,b_y)$ ��ʼ������ѭ�� $M$ ����ɵ�·����ÿ�����趼�� `N`��������`E`��������`S`���ϣ�����`W`�����������У�������Ϊ $x$ �������򣬱�����Ϊ $y$ ������������·�����Ծ�����ͬ�ĵ㡣

��ÿ��ʱ��Σ�FJ ���Բ��ƶ���Ҳ�����������ĵ�·ǰ��һ���������ĸ�����ǡ������һ������������û�е�������·�������λ�ã���Bessie �����������Ƶ�ѡ��

��ÿ��ʱ��㣨�������ӳ�ʼλ�ÿ�ʼ�ĵ�һ���������ǵ����ߵ����ĵ�������������֮������ƽ����

����� FJ �� Bessie �ƻ��ж����ԣ�ʹ˫���ﵽ�����յ�ʱ������޶ȵؼ������ĵ�������������������ĵ���С��������

### �����ʽ

��һ���������� $N$ �� $M$ $(1\le N,M\le 1000)$��

�ڶ����������� $f_x$ �� $f_y$��

�������������� $b_x$ �� $b_y$ $(0\le f_x,f_y,b_x,b_y\le 1000)$��

��һ��Ϊһ������Ϊ $N$ ���ַ��������� FJ ��·����

���һ��Ϊһ������ $M$ ���ַ��������� Bessie ��·����

### �����ʽ

��һ��һ����������ʾ��С������

```input1
2 7
3 0
5 0
NN
NWWWWWN
```

```output1
28
```

