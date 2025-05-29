## ��Ŀ����
You might never have heard of the island group of Iceepeecee, but that suits their inhabitants just fine. Located in a remote part of the South Pacific, they are truly off the beaten track, without any regular air or sea traffic, and they have remained a tropical paradise with unspoiled local fauna and flora.

Being off the map is great when you don't want to be overrun by hordes of tourists, but not so ideal when you actually do need a map for some reason. One such reason came up recently: Iceepeecee's central government needs an exact map of the islands to apportion government funds. Even tropical paradises need money, so Iceepeecee needs a map!

The easiest way to create a map would be an aerial survey. After dismissing chartering planes as too expensive, building an air balloon as too dangerous, and fitting carrier pigeons with cameras as too cruel to animals, they had a brilliant idea. Even with its remote location, there are still plenty of commercial airplanes crossing the skies above Iceepeecee. What if one mounted cameras on flights that are already scheduled to fly anyway? That would be a cheap solution to the problem!

Iceepeecee's plan is to install line-scan cameras on the planes. These cameras point straight downwards and collect images one line segment at a time, orthogonal to the flight path. The photographed line segment will be determined by the altitude that the plane is flying at, and the camera's aperture angle $\theta$ (see Figure F.1). Greater angles $\theta$ mean that the camera can see more, but also that the camera is more expensive.

Moreover, Iceepeecee wants to make sure that each island is observed in its entirety by at least one flight. That means it is not sufficient that an island is only partially photographed by multiple flights, even if the combination of the photographs covers the whole island.

![](https://cdn.luogu.com.cn/upload/image_hosting/99wwtofi.png)

Figure F.1: A view of the plane, shown head-on. Its camera points downward and can see the part of the ground underneath the plane that is shown in green. How much is visible depends on the aperture angle $\theta$.
  
Flight paths follow straight line segments in three-dimensional space, that is, ($x_1, y_1, z_1$) $-$ ($x_2, y_2, z_2$) (see Figure F.2), where the $z$-coordinates give the altitude of the plane. Photographs are taken only along these line segments.

Given the location of their islands and flights, Iceepeecee wants to find the smallest aperture angle $\theta$ that allows for a successful survey. Can you help?

![](https://cdn.luogu.com.cn/upload/image_hosting/3pdn3q1b.png)

Figure F.2: Three islands (shown in black) and two flight paths (red and green). Altitudes are not shown. The shaded areas represent the ground visible on the two flight paths for an optimally chosen $\theta$. This corresponds to the first sample input.Three islands (shown in black) and two flight paths (red and green). Altitudes are not shown. The shaded areas represent the ground visible on the two flight paths for an optimally chosen $\theta$. This corresponds to the first sample input.

## �����ʽ
The input describes a set of islands and flight paths. It starts with a line containing two integers $n$ and $m$, the number $n$ of islands, and the number $m$ of flight paths, respectively ($1 \leq n,m \leq 100$). This is followed by descriptions of the $n$ islands. Each island description starts with a line containing a single integer $n_i$, the number of vertices of the polygon describing the $i^{th}$ island ($3 \leq n_i \leq 100$). It is followed by $n_i$ lines, each containing two integers $x_{ij}$, $y_{ij}$ ($|x_{ij}|, |y_{ij}| \leq 10^6$), specifying the vertices for the $i^{th}$ island in counterclockwise order. Each island's polygon is simple, that is, its vertices are distinct and no two edges of the polygon intersect or touch, other than consecutive edges which touch at their common vertex. Different islands do not intersect or touch.

The input concludes with another $m$ lines, each describing a flight path. Each such line contains six integers $x_1$, $y_1$, $z_1$, $x_2$, $y_2$, $z_2$ ($|x_i|, |y_i|, |z_i| \leq 10^6$, $z_i &gt; 0$ and ($x_1, y_1$) $\neq$ ($x_2, y_2$)). They specify that a flight takes place from ($x_1, y_1, z_1$) to ($x_2, y_2, z_2$).

## �����ʽ
Output the smallest angle $\theta$ (in degrees) that allows for a complete survey of the islands with the given flights. The answer should be exact to an absolute or relative error of $10^{-6}$. If there is no such angle, then output $\texttt{impossible}$. The input is chosen such that if the coordinates of the island vertices are changed by at most $\pm 10^{-8}$, then the answer will not change more than the allowed rounding error.

## ��Ŀ����
��һ���ռ�ֱ������ϵ $O-xyz$��������ƽ�� $xOy$ ���� $n$ ������ÿ������һ���򵥶���Ρ���֤����֮�䲻�ص���

����ϵ���� $m$ ���ɻ����ߣ�������һ���߶Σ������˵������ֱ��� $(x_1,y_1,z_1)$ �� $(x_2,y_2,z_2)$���ɻ�����������һ���ɻ����߷��С�

����Ҫ�ڷɻ���װɨ�������ɨ���������ɨ��ķ�Χȡ���ڽǶ� $\theta$��

�ɻ�λ��һ�� $(x,y,z)$ ʱ�����ǿ����� $(x,y,z)$ Ϊ������һ������Ϊ $2\theta$ �ĵ��������Σ�����������������ڵ��������ƽ�� $xOy$ ��ֱ��ͬʱҲ����ܷɻ����ڵķɻ����ߵ�����ƽ�� $xOy$��ͶӰ��ֱ��
���ɻ�λ�� $(x,y,z)$ ʱ����ɨ�赽���߶ζ���Ϊ������������εĵױߡ�

����һ�����ߣ��串�ǵķ�Χ����Ϊ���ɻ��������������˶�ʱ��������ɨ�赽���߶���ɵ��ı��Ρ�

����С�� $\theta$���Ƕ��ƣ���ʹ��ÿ������������ȫλ��һ�����ߵĸ��Ƿ�Χ�ڡ�������� $\theta$ ȡ��ֵ������������������� `impossible`��

$1\le n,m\le 100$������εı��������� $100$�����и������������ֵ������ $10^6$��

```input1
3 2
3
20 30
50 50
10 50
4
40 20
60 10
75 20
60 30
4
45 60
55 55
60 60
55 65
0 30 20 78 70 5
55 0 20 70 60 10

```

```output1
48.031693036

```

```input2
1 1
4
0 0
10 0
10 10
0 10
5 5 10 15 5 10

```

```output2
impossible

```

