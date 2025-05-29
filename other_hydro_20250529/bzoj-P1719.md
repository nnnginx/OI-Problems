## ��Ŀ����
Farmer John is quite the nature artist: he often constructs large works of art on his farm. Today, FJ wants to construct a giant "field web". FJ's field is large convex polygon with fences along the boundary and fence posts at each of the $n$ corners $(1 \le  n \le  150)$. To construct his field web, FJ wants to run as many ropes as possible in straight lines between pairs of non-adjacent fence posts such that no two ropes cross. There is one complication: FJ's field is not completely usable. Some evil aliens have created a total of $g\ (0 \le  g \le  100)$ grain circles in the field, all of radius $r\ (1 \le  r \le  10^5)$. FJ is afraid to upset the aliens, and therefore doesn't want the ropes to pass through, or even touch the very edge of a grain circle. Note that although the centers of all the circles are contained within the field, a wide radius may make it extend outside of the field, and both fences and fence posts may be within a grain circle. Given the locations of the fence posts and the centers of the circles, determine the maximum number of ropes that FJ can use to create his field web. FJ's fence posts and the circle centers all have integer coordinates $x$ and $y$ each of which is in the range $0\dots 10^6$.

Լ������һ����Ȼ��������ʦ������������������ϴ���һЩ�޴���������������죬�����������ϴ���һ�����������ɵľ޻�������������һ������Σ��� $n$ �����׮��֮������Χ�ɡ�Ϊ�˴������ľ޻����������þ��������������������ֱ���������������ڵ����׮������Ϊ�˻��������������������������ý��档

Լ����һ���Ѵ���һЩа��������������������������� $g$ ����Ȧ����Щ��Ȧ����һ���İ뾶 $r$���������������ˣ����Բ������κ�����ͨ����Щ��Ȧ����ʹ������Ȧ�ı߼�Ҳ���С���Щ��Ȧ��Բ�Ķ�������֮�ڣ���һЩ��Ȧ�����в���������֮�⡣һЩ��ʻ������׮���п�����ĳһ����Ȧ��������׮�͹�Ȧ�����꣬�������������������е����궼�� $[0,10^6]$ �ڵ�������
## �����ʽ
* Line $1$: Three space-separated integers: $n,g$, and $r$. 
* Lines $2\dots n+1$: Each line contains two space-separated integers that are the $x,y$ position of a fence post on the boundary of FJ's field. 
* Lines $n+2\dots n+g+1$: Each line contains two space-separated integers that are the $x,y$ position of a circle's center inside FJ's field.
 
�� $1$ �������������� $n,g,r$�������� $n$ ��ÿ����������������ʾ���׮�����ꡣ������ $g$ ��ÿ����������������ʾһ����Ȧ��Բ�����ꡣ

## �����ʽ
* Line $1$: A single integer that is the largest number of ropes FJ can use for his artistic creation.

������������

```input1
5 3 1
6 10
10 7
9 1
2 0
0 3
2 2
5 6
8 3
```
```output1
1
```
## ����˵��

A pentagonal field, in which all possible ropes are blocked by three grain circles, except for the rope between fenceposts $2$ and $4$.

�������׮ $2$ �� $4$ ֮���������������������ᾭ����Ȧ��
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1\le n\le 150$��$0\le g\le 100$��$1\le r\le 10^5$��$x_i,y_i\in [0,10^6]$��
## ��Ŀ��Դ
Gold