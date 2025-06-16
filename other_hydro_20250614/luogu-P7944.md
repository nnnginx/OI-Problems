## ��Ŀ����

**This is an interactive problem.**


Ran is helping Yukari to maintain the border of Gensokyo. 

The border of Gensokyo is a $n\times m$ matrix, where $n$ and $m$ are both even. Unfortunately, due to Moriya Shrine's moving in, there are now $4$ weakened points within the matrix.

To ease the maintenance work, Ran have already found a path from $(1,1)$ to $(n,m)$, going only down or right. The path separates the four weakened points so that exactly two of them are on either side. She will tell you this path in the input.

Now you need to help Ran maintain the border. You can use the operation `? x y` to ask whether the point $(x,y)$ is weakened. And after the query, Ran will mark the point with blue.

If, after a query, you have just found out the $k$-th weakened point, and $k$ is even, you will need to construct a simple path from the $(k-1)$-th weakened point to the $k$-th. The path you constructed must pass through and only pass through **all** the points that are marked blue.  Ran will then strengthen these points in the border and recolor them red.

Ran does not want to do repetitive work, so you can only ask for points that are white with the `?` query.

Now Ran hopes that you can ask all the "weakened points" and finish all the constructions.

### Interaction Protocol

First read two integers $n$ and $m$ from standard input.

Then read several points (including start and end points) from standard input, one per line, representing a simple path from $(1,1)$ to $(n,m)$.

Then you can make **unlimited** queries. Print your queries to standard output in the format of `? x y`. You will then receive an integer $p$ from standard input. If $p=1$, it means that the point you asked is indeed weakened; if $p=0$, it means that it is not weakened.

Remember to flush your output, you can use `fflush(stdout);` in C++. Please refer to your programming language's documentation.

On the $k$-th time ($k$ is even) of receiving the result $p=1$, please output several points (including the two weakened points) in order, one per line, ending with $-1,-1$, so that they represent the simple path from the $(k-1)$-th to the $k$-th weakened point.

You need to exit your program immediately after finding the fourth weakened point and finishing the construction.


## �����ʽ
Refer to "Interactive Method".

## �����ʽ
Refer to "Interactive Method".

## ��Ŀ����
**����һ�������⡣**

��һ�� $n\times m$ �ľ��󣬱�֤ $n$ �� $m$ **��Ϊż��**����ʼ���и��Ӷ��ǰ�ɫ���� $(x,y)$ ��ʾ����� $x$ �е� $y$ �еĸ��ӡ�

���������ĸ��ؼ��㣨Ҳ��������ĸ��ӣ������ұ�֤����һ���� $(1,1)$ �� $(n,m)$ ��ֻ�����»����ҵ�·�������ĸ��ؼ���ָ�������ÿ��������**·���ѱ�������**

������ò��� `? x y` ��ѯ�ʸ��� $(x,y)$ �Ƿ�Ϊ�ؼ��㣨�ǵĻ����������� $1$�����򷵻� $0$��������ѯ�ʹ���ø��ӻᱻȾ����ɫ��

�����ż����ѯ�ʵ��ؼ��������Ҫ���һ���ӵ����ڶ��α�ѯ�ʵ��Ĺؼ��㵽���һ��ѯ�ʵ��Ĺؼ���ļ�·�������㾭���ҽ�����**����**��Ⱦ����ɫ�ĸ��ӡ������ɺ����е���ɫ���Ӷ����ɺ�ɫ��

��Ҫע�⣬��**ֻ��ѯ�ʰ�ɫ����**��

```input1
4 4
1 1
1 2
2 2
3 2
3 3
3 4
4 4

0

1

0

0

1







1

1

```

```output1








? 2 2

? 2 1

? 3 1

? 3 2

? 4 1

2 1
2 2
3 2
3 1
4 1
-1 -1
? 1 4

? 1 3

1 4
1 3
-1 -1

```

## ��ʾ
### Explanation

The matrix in the sample is as follows:

```plain
..XX
X...
....
X...
```

Which `X` means a "weakened point".

### Constraints

$4\le n,m\le100$��

