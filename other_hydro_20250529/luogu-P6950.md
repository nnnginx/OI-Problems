## ��Ŀ����


A well-known puzzle is to `tour` all the squares of an $8 \times 8$ chessboard using a knight, which is a piece that can move only by jumping one square in one direction and two squares in an orthogonal direction. The knight must visit every square of the chessboard, without repeats, and then return to its starting square. There are many ways to do this, and the chessboard size is manageable, so it is a reasonable puzzle for a human to solve.

However, you have access to a computer, and some coding skills! So, we will give you a harder version of this problem on a rectangular $m \times n$ chessboard with an additional constraint: the knight may never cross its own path. If you imagine its path consisting of straight line segments connecting the centers of squares it jumps between, these segments must form a simple polygon; that is, no two segments intersect or touch, except that consecutive segments touch at their common end point. This constraint makes it impossible to visit every square, so instead you must maximize the number of squares the knight visits. We keep the constraint that the knight must return to its starting square. Figure J.1 shows an optimal solution for the first sample input, a $6 \times 6$ board.

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15698/1.png)

Figure J.1 : An optimal solution for a $6 \times 6$ board.



## �����ʽ


The input consists of a single line containing two integers $m (1 \le m \le 8)$ and $n (1 \le n \le 10^{15}),$ giving the dimensions of the rectangular chessboard.



## �����ʽ


Display the largest number of squares that a knight can visit in a tour on an $m \times n$ chessboard that does not cross its path. If no such tour exists, display $0$ .



## ��Ŀ����
### ��Ŀ����

���� $m$ $\times$ $n$ ��С�ľ�����������Ծ�������֣������������һ�㿪ʼ���ڱ�֤�����ʡ�������£�����ྭ���������ӣ�������㣬���յ㲻�㣩�����Իص���ʼ�㣿

�����ʡ����������·����ֱ�߶���ɣ���Щֱ�߶�������������Ծ�������ε����ģ���ͼ������Щֱ�߶α����γ�һ���򵥵Ķ���Ρ�Ҳ����˵��û�������߶��ཻ��Ӵ������������߶����乫���˵㴦�Ӵ���

### �����ʽ

һ�У����������� $m$ $(1 \le m \le 8)$ �� $n$ $(1 \le n \le 10^{15})$��

### �����ʽ

һ�У�����ྭ���ĸ�������
��û��������·������� $0$ ��

```input1
6 6

```

```output1
12

```

```input2
8 3

```

```output2
6

```

```input3
7 20

```

```output3
80

```

```input4
2 6

```

```output4
0

```

## ��ʾ
Time limit: 2 s, Memory limit: 1024 MB. 



