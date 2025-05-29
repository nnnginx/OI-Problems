## ��Ŀ����
A simple polygon with $N$ vertices is drawn on an infinite rectangular grid. For such a polygon, only neighboring edges touch at their common vertex; no other of its edges intersect or touch. All vertices of the polygon lie on grid points, i.e., vertices have integer coordinates.

Your task is to find the total length of grid line segments which lie strictly inside the given polygon (these line segments are highlighted in the drawings below).

## �����ʽ
The first line of input contains a single integer $N$, the number of vertices of the polygon. Each of the following $N$ lines contains two integers $x$ and $y$, the coordinates of one vertex. The vertices are given either in clockwise or counterclockwise order. All vertices are distinct, but more than two consecutive vertices may lie on a line.

## �����ʽ
The only line of output must contain a decimal number: the total length of grid line segments which lie strictly inside the given polygon.

## ��Ŀ����
��ƽ��ֱ������ͼ����һ���򵥶���Σ����� $N$ �����㣬ÿ�����㶼�ڸ���ϣ����=���㣩��  
�����ϸ��ڶ�����ڲ����������ж೤���ڡ��������͡��У� �ϸ��ڶ�����ڲ��������߽���Ӵ���ʾ��  
��ע�⾫�ȡ�����Ĵ�Ϊ $L$����׼��Ϊ $R$����ֻ������ $|L - R| \le R \times 10^{-6}$ �� $|L - R| <= 10^{-6}$ ���������е�����һ�����ɵ÷֡�

### ��������
��һ����һ������ $N$��  
�ڽ������� $N$ ���У�ÿ���������� $x$ �� $y$����ʾһ����������ꡣ

### �������
�����һ�У�һ��������ʾ�ϸ��ڶ�����ڲ��������ߵĳ��ȡ�

#### �������� 1
![](https://cdn.luogu.org/upload/pic/42607.png)

����Ҫ��ĺ���֮��Ϊ $\frac{4}{3} + \frac{8}{3} =4$������֮��Ϊ $3+2+1=6$���ܳ� $4+6=10$��

#### �������� 2
![](https://cdn.luogu.org/upload/pic/42608.png)

����Ҫ��ĺ���֮��Ϊ $1+2+4=7$������֮��Ϊ $\frac{9}{4}+\frac{3}{2}+\frac{7}{4}=5.5$���ܳ� $7+5.5=12.5$��

�����ṩ�ߣ�Planet6174

```input1
3
5 1
2 4
1 1
```

```output1
10.0
```

```input2
5
0 0
-2 2
-2 -1
2 -2
2 0
```

```output2
12.5
```

## ��ʾ
**Sample Explanation 1**

The length of horizontal lines is $\frac{4}{3} + \frac{8}{3} = 4$. The length of vertical lines is $3 + 2 + 1 = 6$. The total length is $4 + 6 = 10$.

**Sample Explanation 2**

The length of horizontal lines is $1+2+4 = 7$. The length of vertical lines is $\frac{9}{4}+\frac{3}{2}+\frac{7}{4} = 5.5$. The total length is $7 + 5.5 = 12.5$.

**���ݷ�Χ**

���� $50\%$ �����ݣ���������еı߾����������ϡ�

�����������ݣ�$3 \le N \le 10^5,-5 \times 10^8 \le x,y \le 5 \times 10^8$��

