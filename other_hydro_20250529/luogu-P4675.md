## ��Ŀ����
In the capital of Byteland, there is a fenced park whose area is a rectangle. The trees and the visitors in the park are represented as circles.

There are four entrances in the park, one in each corner (1 = bottom-left, 2 =bottom-right, 3 = top-right, 4 = top-left). The visitors can enter and exit the park only through the entrances.

Visitors can enter and exit the park when they touch both sides of a corner of the corresponding entrance. Visitors can move freely in the park, but they cannot overlap any of the trees or the fence.

Your task is to calculate for each visitor, given the entrance they will enter the park,through which entrances they can exit the park.

## �����ʽ
The first input line contains two integers $w$ and $h$ : the number of trees in the park and the number of visitors.

The second input line contains two integers $w$ and $h$ : the width and the height of the park area. The bottom-left corner is $(0,0)$, and the top-right corner is $(w,h)$.

After this, there are  lines that describe the trees. Each line contains three integers, $x,y$ and $r$ : the center of the tree is $(x,y)$ and its radius is $r$. The trees do not overlap each other or the fence.

Finally, there are $m$ lines that describe the visitors. Each line contains two integers $r$ and $e$ : the radius of the visitor and the entrance they will enter the park.

In addition, no tree overlaps a square area of $2k\times2k$ in each corner, where $k$ is the radius of the largest visitor.

## �����ʽ
You should output for each visitor a single line containing the entrances through which they can exit the park, in sorted order without spaces in between.

## ��Ŀ����
## ��Ŀ����

�� Byteland ���׶�����һ����Χǽ�����ľ��ι�԰��������Բ�α�ʾ�οͺ�����  
��԰�����ĸ���ڣ��ֱ����ĸ����䣨$1, 2, 3, 4$ �ֱ��Ӧ���¡����¡����ϡ����ϣ����ο�ֻ�ܴ���ڽ�����  
�οͿ����������빫԰�����ڱ����е�ʱ�������Ӧ����ڡ��οͿ����ڹ�԰�����ɻ�������������ص���  
���������Ϊÿ���οͼ��㣬�������ǽ��빫԰����ڣ����ǿ��Դ��ĸ�����뿪��԰��

## �����ʽ

��һ�а����������� $n$ �� $m$���ֱ�Ϊ���ĸ������ο͵ĸ�����  
�ڶ��а����������� $w$ �� $h$����԰�����½��� $(0,0)$�����Ͻ��� $(w,h)$��  
������ $n$ �У�ÿ���������� $x,y$ �� $r$����ʾ��һ��Բ���� $(x,y)$ �Ұ뾶Ϊ $r$ ��������֤������֮�䲻�ụ���ص���  
������ $m$ �У�ÿ���������� $r$ �� $e$����ʾ��һ���뾶Ϊ $r$ ���οʹ���� $e$ ���롣  
���⣬��֤û��������ÿ�������һ����СΪ $2k^2$ �ķ��������ص���$k$ ��ʾ�����οͰ뾶��

## �����ʽ

����ÿ���οͣ����û�пո��һ�У���ʾ���οͿ��Դ��⼸������뿪�������������С�

## ��������ʾ

�����������ص�����Ϊ���ǲ�ֹһ�������㡣

��ͼչʾ��ÿ���ο͵���ںͿ��ܵ�·�ߣ�

![](https://i.loli.net/2018/08/11/5b6e30c4b5a35.png)

����ÿ��������$4k \leq w,h \leq 10^9$��$k$��ʾ�����οͰ뾶��

|������|����|���ݷ�Χ|
|:-:|:-:|-|
|1|27|$1 \leq n \leq 2000,m=1$|
|2|31|$1 \leq n \leq 200,1 \leq m \leq 10^5$|
|3|42|$1 \leq n \leq 2000,1 \leq m \leq 10^5$|

�� @I_love_him52 �ṩ����

```input1
5 3
16 11
11 8 1
6 10 1
7 3 2
10 4 1
15 5 1
1 1
2 2
2 1

```

```output1
1234
2
14

```

## ��ʾ
Two objects touch if they have one common point. Two objects overlap if they have more than one common point.

## ��������

The following figure shows the entrance areas and possible routes for each visitor:

![](https://cdn.luogu.com.cn/upload/pic/20869.png)

## Subtasks

In all subtasks $4k\leq w,h\leq10^9$ where $k$ is the radius of the largest visitor.

### Subtask 1 (27 points)

- $1\leq n\leq2000$

- $m=1$

### Subtask 2 (31 points)

- $1\leq n\leq200$

- $1\leq m\leq10^5$

### Subtask 3 (42 points)

- $1\leq n\leq2000$

- $1\leq m\leq10^5$


