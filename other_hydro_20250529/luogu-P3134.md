## ��Ŀ����
Farmer John has installed a fancy new milking machine in his barn, but it draws so much power that it occasionally causes the power to go out! This happens so often that Bessie has memorized a map of the barn, making it easier for her to find the exit of the barn in the dark. She is curious though about the impact of power loss on her ability to exit the barn quickly. For example, she wonders how much farther she might need to walk find the exit in the dark.


The barn is described by a simple (non self-intersecting) polygon with integer  vertices $(x_1, y_1) \ldots (x_n, y_n)$ listed in clockwise order.  Its edges alternate between horizontal (parallel to the x-axis) and vertical (parallel to the y-axis); the first edge can be of either type. The exit is located at

$(x_1, y_1)$.  Bessie starts inside the barn located at some vertex  $(x_i, y_i)$ for $i > 1$.  She can walk only around the perimeter of the barn, either clockwise or counterclockwise, Her goal is to travel a minimum distance to reach the exit. This is relatively easy to do with the lights on, of course, since she will travel either  clockwise or counterclockwise from her current location to the  exit -- whichever direction is shorter.


One day, the lights go out, causing Bessie to panic and forget which vertex she is standing at.  Fortunately, she still remembers the exact map of the barn, so she can possibly figure out her position by walking around and using her sense of touch.  Whenever she is standing at a vertex (including at her initial vertex), she can feel the exact interior angle at that vertex, and she can tell if that vertex is the exit.  When she walks along an edge of the barn, she can determine the exact length of the edge after walking along the entire edge.  Bessie decides on the following strategy: she will move clockwise around the perimeter of the barn until she has felt enough angles and edges to deduce the vertex at which she is currently located.  At that point, she can easily figure out how to get to the exit by traveling a minimum amount of remaining distance, either by continuing to move clockwise or by switching direction and moving counter-clockwise.


Please help Bessie determine the largest amount by which her travel distance will increase in the worst case (over all possibilities for her starting vertex) for travel in the dark versus in a lit barn.


## �����ʽ
The first line of the input contains $N$ ($4 \leq N \leq 200$).  Each of the next $N$ lines contains two integers, describing the points $(x_i, y_i)$ in clockwise order around the barn.  These integers are in the range $-100,000 \ldots 100,000$.


## �����ʽ
Output the largest amount that Bessie's travel distance will increase in the

worst case starting position using the strategy in the problem statement.


## ��Ŀ����
### ��Ŀ����

Farmer John �����ĹȲ��ﰲװ��һ���ǳ�������¼��̻���������̨���̻��ĵ�̫���ˣ���ʱ����ùȲ�ֱ��ͣ�磡�����·�����̫Ƶ���ˣ������� Bessie ֱ�ӰѹȲֵĵ�ͼ�����ˣ��Ա��ڿ����ںڰ����ҵ��Ȳֵĳ��ڡ�������ͣ������������뿪�Ȳֵ�������Ӱ��ǳ����档����˵������֪�����ںڰ�����Ҫ�߶�Զ���ҵ��Ȳֵĳ��ڡ�

�Ȳ����·���Ա�����Ϊ��һ���򵥵��ü�����������ʾ�Ķ���Σ���Щ������԰���˳ʱ�뱻��ʾΪ $(x_1, y_1) \cdots (x_n, y_n)$����֤��Щ�������ɵ���û�н�������������Щ�㹹�ɵı���ˮƽ�ᣨƽ���� $x$ �ᣩ����ֱ�ᣨƽ���� $y$ �ᣩ֮�佻����֡���һ���߿���������һ�����͡��Ȳֳ��������� $(x_1, y_1)$ ��Bessie �ӹȲ�������һ���� $(x_i, y_i)$ ��ʼ�ߡ���ֻ����������Щ���ߣ�Ҫ��Ȼ��˳ʱ�룬Ҫ��Ȼ������ʱ�룬����Ŀ���������̾���ִ���ڡ���Ȼ����������ŵĻ�����»�����Լ򵥣���Ϊ��Ҫ��Ȼ˳ʱ��Ҫ��Ȼ��ʱ���ߣ�����ν�ĸ������·�̸���һ�㡣

һ�죬�Ȳ�ͻȻͣ���ˣ����� Bessie �ܵ����š���������վ���ĸ����㡣�ҿ������ǵùȲֵ�׼ȷ��ͼ�������������Ĵ����ߣ������Ĵ�����Ū�������λ�á�����ʲôʱ��ֻҪ��վ��һ�����㣬��ô���Ϳ��Ը��ܵ����������ĳ���Ƕȣ�Ū���������ǲ��ǳ��ڡ��������ŹȲֵ�һ���������ʱ�������������ȷ�ı߳���Bessie ��������ôһ�����ԣ�����˳ʱ�����ŹȲ���Χ�ı��ߣ�ֱ����֪�����㹻�ĽǶȺͱߡ������ƶϳ���Ŀǰ�ڵ����ĸ����㡣���Ǹ����㣬���Ϳ������׵�Ū�����������̾��뵽����ڣ�Ҫ��Ȼ��������˳ʱ���ߣ�Ҫ��Ȼ����ȥ������ʱ���ߣ���

����� Bessie ��������������κ�һ����������£����������£����ںڰ��к����ŵƵ�ʱ�򵽴���ڵľ���Ĳ�ֵ�����ҵ���ֵ�����ֵ����

### �����ʽ

��һ�а���һ������ $N (4 \leqslant N \leqslant 200)$ �������� $N$ �У�ÿ�а����������֣�����˳ʱ���ʾ���� $(x_i, y_i)$��$x_i, y_i \in [-10^5, 10^5]$ ��

### �����ʽ

��� Bessie ���������£����ںڰ��к����ŵƵ�ʱ�򵽴���ڵľ���Ĳ�ֵ�����ҵ���ֵ�����ֵ����

### ˵��/��ʾ

����������У�Bessie ��ʼ���Ըо��������� $90 \degree$ ��վ�ţ���������𲻳��������� $2, 3, 4$ �е���һ�����㡣

������һ�����Ժ�Bessie Ҫ��Ȼ���˳���Ҫ��Ȼ�Ϳ��Ը������߹��ľ����ƶϳ�����λ�á�������£�

������� $2$ �ŵ㿪ʼ�ߣ�����Ҫ�ںڰ����� $12$ ����λ������һ����λ����������㡢ʮһ����λ�뿪�Ȳ֡�ͬʱ��������ŵƣ�������ֻ�� $10$ ����λ���뿪�Ȳ֡���ֵ�� $2$ ��

����� $3$ �ŵ㿪ʼ�������������Ҫ�� $11$ ����λ��

����� $4$ �ŵ㿪ʼ�������������Ҫ�� $1$ ����λ��

����������ֵ�� $2$ ��

```input1
4
0 0
0 10
1 10
1 0
```

```output1
2
```

## ��ʾ
In this example, Bessie can feel that she is initially standing at a 90-degree angle, but she cannot tell if she is initially standing at vertex 2, 3, or 4.

After taking a step along one edge in the clockwise direction, Bessie either reaches the exit or can uniquely determine her location based on the length of this edge. The distances she obtains are:

If starting at vertex 2: she travels 12 units in the dark (1 unit to reach vertex 3, then 11 units to continue to the exit). She only needs to travel 10 units in a lit barn. This is an extra distance of 2 for this vertex.

If starting at vertex 3: she travels 11 units in both cases.

If starting at vertex 4: she travels 1 unit in both cases.

The worst-case difference over all starting points is therefore 12 - 10 = 2.  That is, Bessie can guarantee that using her strategy, no matter where she starts, she will travel at most 2 extra units of distance farther in the dark than in the light.


