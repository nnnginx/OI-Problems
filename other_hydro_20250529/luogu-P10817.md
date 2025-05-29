## ��Ŀ����
Prof. Pang enters a trap room in a dungeon. The room can be represented by an $n$ by $m$ chessboard. We use $(i, j)$ ($1\le i\le n$, $1\le j\le m$) to denote the cell at the $i$-th row and $j$-th column. Every second, the floor of one cell breaks apart (so that Prof. Pang can no longer stand on that cell.) After $nm$ seconds, there will be no cell to stand on and Prof. Pang will fall through to the next (deeper and more dangerous) level.

But Prof. Pang knows that calm is the key to overcome any challenge. So instead of being panic, he calculates the number of rectangles such that every cell in it is intact (i.e., not broken) after every second. (A rectangle represented by four integers $a, b, c$ and $d$ ($1\le a\le b\le n, 1\le c\le d\le m$) includes all cells $(i, j)$ such that $a\le i\le b, c\le j\le d$. There are $
\frac{n(n+1)}{2} \times \frac{m(m+1)}{2}$ rectangles in total.)

## �����ʽ
The first line contains two integers $n$, $m$ ($1\le n, m\le 500$) separated by a single space. 

The $(i+1)$-th line contains two integers $a$, $b$ separated by a single space representing that the cell $(a, b)$ breaks apart at the $i$-th second. It is guaranteed that each cell appears exactly once in the input. 

## �����ʽ
Output $nm$ lines. The $i$-th line should contain the number of rectangles such that every cell in it is intact after the first $i$ cells break apart.

## ��Ŀ����
### ��Ŀ����

�ӽ��ڽ�����һ�����³ǵ����巿�䡣������������һ�� $n$ �� $m$ �е���������ʾ�������� $(i, j)$ ($1\le i\le n$, $1\le j\le m$) ����ʾ�� $i$ �е� $j$ �еĵ�Ԫ��ÿ���ӣ���һ����Ԫ��ĵذ�����ѣ������ӽ��ھͲ�����վ�������Ԫ�����ˣ������� $nm$ ��󣬽�û�е�Ԫ��ɹ�վ�����ӽ��ڽ����䵽��һ���������Ҹ�Σ�յģ��㼶��

���ӽ���֪���侲�ǿ˷��κ���ս�Ĺؼ�����ˣ���û�о��ţ����Ǽ�������ÿ���Ӻ����е�Ԫ����õľ��ε�����������ÿ����Ԫ���ھ����ж�û�����ѣ���һ���������ĸ����� $a, b, c$ �� $d$ ($1\le a\le b\le n, 1\le c\le d\le m$) ��ʾ���������� $(i, j)$ ʹ�� $a\le i\le b, c\le j\le d$���ܹ��� $
\frac{n(n+1)}{2} \times \frac{m(m+1)}{2}$ �����Ρ�

### �����ʽ

��һ�а����������� $n$, $m$ ($1\le n, m\le 500$)���ÿո�ָ���

�� $(i+1)$ �а����������� $a$, $b$����ʾ�ڵ� $i$ ���ӵ�Ԫ�� $(a, b)$ ���ѡ���֤ÿ����Ԫ���������г���ǡ��һ�Ρ�

### �����ʽ

��� $nm$ �С��� $i$ ��Ӧ������ǰ $i$ ����Ԫ������֮��ÿ����Ԫ����õľ��ε�������

### ��ʾ

��ʾ���У��ڵ�һ����� $3$ �����Ϊ $1$ �ľ��κ� $2$ �����Ϊ $2$ �ľ���������������˵�һ��Ӧ����� $5$���ڵڶ���󣬽��ڶ����еĵ�Ԫ�񱣳���á���Ӧ���� $3$���ڵ�����󣬽�һ����Ԫ�񱣳���á���Ӧ���� $1$���ڵ���������е�Ԫ�����ѣ����Դ�Ӧ���� $0$��

�����ߣ�[Immunoglobules](https://www.luogu.com.cn/user/1066251)

```input1
2 2
1 1
2 1
1 2
2 2
```

```output1
5
3
1
0
```

## ��ʾ
In the example, after the first second, there are $3$ rectangles of area $1$ and $2$ rectangles of area $2$ that satisfy the constraint. So the first line should contain a $5$. After the second second, only cells in the second column remains intact. The answer should be $3$. After the third second, only one cell remains intact. The answer should be $1$. After the fourth second, all cells broke apart so the answer should be $0$. 

