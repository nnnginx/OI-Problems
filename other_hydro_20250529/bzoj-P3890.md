## ��Ŀ����

Bessie and her sister Elsie want to travel from the barn to their favorite field, such that they leave at exactly the same time from the barn, and also arrive at exactly the same time at their favorite field. The farm is a collection of $n$ fields numbered $1$..$n$, where field $1$ contains the barn and field $n$ is the favorite field. The farm is built on the side of a hill, with field $X$ being higher in elevation than field $Y$ if $X < Y$. An assortment of $m$ paths connect pairs of fields. However, since each path is rather steep, it can only be followed in a downhill direction. For example, a path connecting field $5$ with field $8$ could be followed in the $5 \to 8$ direction but not the other way, since this would be uphill. It might take Bessie and Elsie different amounts of time to follow a path; for example, Bessie might take $10$ units of time, and Elsie $20$. Moreover, Bessie and Elsie only consume time when traveling on paths between fields -- since they are in a hurry, they always travel through a field in essentially zero time, never waiting around anywhere. Please help determine the shortest amount of time Bessie and Elsie must take in order to reach their favorite field at exactly the same moment.

**���룺**

Bessie �� Elsie ���ũ������� $1$ ����� $n$��ũ���� $n$ ���� $1\cdots n$ ����ع��ɡ�

ũ������ɽ�ϣ�������� $X<Y$��������� $X$ ����صĸ߶ȸ��ڵ� $Y$ ����ء���ũ���У��� $m$ ����·����ͬ���������������

����������ɽ·���ͣ���ЩС·ֻ������**�Ӹߵ���**�ķ����ߡ����磬һ�����ӵ� $5$ ����غ� $8$ ����ص�С·ֻ������ $5\to 8$ �ķ����ߣ��������������������������֮�����ֻ��һ��С·��

Bessie �� Elsie ��ͬһ��С·���ܻỨ�Ѳ�ͬ��ʱ�䡣���磬ͨ��ͬһ��С·��Bessie ���ܻ�ķ� $10$ ����λ��ʱ�䣬�� Elsie ��ķ� $20$ ����λ��ʱ�䡣

���⣬����ֻ����ͨ��С·ʱ�ķ�ʱ�䡣�ڴ������ʱ����ķ�ʱ�䣬Ҳ����ͣ�����ȴ���

�ʣ� Bessie �� Elsie ͬʱ��������ͬʱ������� $n$ ����̵�ʱ�䡣

## �����ʽ

The first input line contains $n$ and $m$, separated by a space.

Each of the following $m$ lines describes a path using four integers $a,b,c,d$, where $a$ and $b$ (with $a < b$) are the fields connected by the path, $c$ is the time required for Bessie to follow the path, and $d$ is the time required for Elsie to follow the path.

��һ���������� $n,m$���ÿո�ֿ���

������ $m$ �У�ÿ���ĸ����� $a,b,c,d$������ $a,b(a<b)$ ��ʾ����������С·���ӵ���أ�$c$ ��ʾ Bessie ͨ������С·��ʱ�䣬 $d$ ��ʾ Elsie ͨ������С·��ʱ�䡣

## �����ʽ

A single integer, giving the minimum time required for Bessie and Elsie to travel to their favorite field and arrive at the same moment. If this is impossible, or if there is no way for Bessie or Elsie to reach the favorite field at all, output the word `IMPOSSIBLE` on a single line.

һ����������ʾ����ͬʱ������ͬʱ��������ʱ�䡣����޷�ͬʱ������ `IMPOSSIBLE`��

```input1
3 3
1 3 1 2
1 2 1 2
2 3 1 2
```

```output1
2
```

## ����˵��

Bessie is twice as fast as Elsie on each path, but if Bessie takes the path $1\to 2 \to 3$ and Elsie takes the path $1\to 3$ they will arrive at the same time.

Bessie ��ÿһ��·���� Elsie ��������

�� Bessie ���� $1\to 2\to 3$ ��·�ߣ�Elsie ���� $1\to 3$ ��·�ߣ����ǿ���ͬʱ���

## ���ݹ�ģ��Լ��

 ���� $100\%$ �����ݣ�$1 \le n \le 100$��$m \le \frac{n\times (n-1)}{2}$��$1\le c,d\le 100$��

## ��Ŀ��Դ

Silver