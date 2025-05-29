## ��Ŀ����
Blue-edged Shot is forbidden from playing Genshin Impact by LeavingZ. However, today LeavingZ went to Huazhong University of Science and Technology, School of Cyber Science and Engineering, to harvest the gold medal of the 2024 International Collegiate Programming Contest in Hubei Province, China.

An activity of Genshin Impact called `Dodoco's Bomb-Tastic Adventure` has begun. This is a single-player game, where each game involves a pond. The pond can be divided into an $n$ by $m$ grid, with the cell in the $i$-th row and $j$-th column represented by $(i,j)$. Among these, $k$ cells contain fish, and you will play as the Spark Knight Klee, who fishes with explosives.

![](https://cdn.luogu.com.cn/upload/image_hosting/3keap2xe.png)

If Klee drops a bomb at $(a,b)$, all the cells $(x,y)$ satisfying $|x-a|+|y-b|\le 1$ will be covered by the explosion. For every cell covered by the explosion, Klee will catch one fish from it. Klee can drop bombs at any location. The question is, to catch all the fish, how many `Jumpy Dumpty` bombs are needed at a minimum?

## �����ʽ
The first line contains three integers $n,m,k$ ($1 \le n,m \le 10^3, 1 \le k \le 10$) --- the size of the grid and the number of cells containing fish.

The following $k$ lines, each line contains three integers $x_i,y_i,a_i$ ($1\le x_i \le n, 1 \le y_i \le m, 1 \le a_i \le 3$), representing there are $a_i$ fish in cell $(x_i,y_i)$.

It is guaranteed that the input cell $(x_i,y_i)$ are unique.

## �����ʽ
Output a single integer, denoting the minimum number of bombs needed.

## ��Ŀ����
### ��Ŀ����
��Blue-edged Shot �� LeavingZ ��ֹ�桶ԭ�񡷡�Ȼ�������� LeavingZ ǰ���˻��пƼ���ѧ�������ѧ�빤��ѧԺ���μ�2024���й�����ʡ���ʴ�ѧ��������ƾ��������ջ��˽��ơ�

��ԭ���е�һ������ը����ð���Ѿ���ʼ�ˡ�����һ��������Ϸ��ÿ����Ϸ���漰һ���������������Ա�����Ϊһ�� $n��m$ ���������е� $i$ �е� $j$ �еĵ�Ԫ���ʾΪ $(i,j)$������Щ��Ԫ���У��� $k$ ����Ԫ������㣬�㽫���ݻ���ʿ����������ըҩ�����㡣

��������� $(a,b)$ λ��Ͷ��ը������ô��������$|x-a|+|y-b|\le 1$�ĵ�Ԫ�� $(x,y)$ ��������ը���ǡ�����ÿһ������ը���ǵĵ�Ԫ�񣬿�����������в���һ���㡣�����������κ�λ��Ͷ��ը���������ǣ�Ϊ�˲������е��㣬������Ҫ����ö`�ı�ը��`����
### �����ʽ
��һ�а����������� $n,m,k$ ($1 \le n,m \le 10^3, 1 \le k \le 10$)���ֱ��ʾ����Ĵ�С���������������Լ�������ĵ�Ԫ��������

�������� $k$ �У�ÿ�а����������� $x_i,y_i,a_i$ ($1\le x_i \le n, 1 \le y_i \le m, 1 \le a_i \le 3$)����ʾ������� ($x_i, y_i$) ��Ԫ������ $a_i$ ���㡣

���뱣֤���е� $(x_i, y_i)$ ��Ԫ�����궼��Ψһ�ġ�
### �����ʽ
���һ����������ʾ���������ը���������� ����������У�����Ҫ���㲢���һ������������������Ϊ�˲�������������Ͷ�ŵ����١��ı�ը����������
### ���� #1

#### �������� #1

```
5 5 3
1 1 2
2 2 1
5 5 2
```

#### ������� #1

```
4
```
### ��ʾ

һ�ֿ��ܵķ������� $(1,2)$ λ��Ͷ����öը�������� $(5,5)$ λ��Ͷ��������öը����

����֤��û�б�����𰸸�С�Ľ⡣

```input1
5 5 3
1 1 2
2 2 1
5 5 2
```

```output1
4
```

## ��ʾ
One possible way is to drop two bombs at $(1,2)$ and another two at $(5,5)$.

It can be proven that there is no solution with a smaller answer.

