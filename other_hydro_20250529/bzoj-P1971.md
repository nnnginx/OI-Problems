## ��Ŀ����

Byteotian ������������׼���з�һ��������������������ǿ��ٵ��ҳ���������֮�䲻ͬ��·������������������ҳ���̵�·���Ļ����ǲ��ѵġ����ǲ��ҵ��ǣ�������ʱ����֪���� $k$ �̵�·�������ҳ���֮�⣬·�����Ի����ظ�������������ġ������������֮���� $4$ ��·�������ǵĳ��ȷֱ��� $2,4,4,5$����ô���·���ĳ���Ϊ $2$���γ�Ϊ $4$��������Ϊ $4$�����ĳ��ĳ���Ϊ $5$��

## �����ʽ

In the first line of the standard input there are two positive integers $n$ and $m$, separated by a single space. They are the number of towns in Byteotia and the number of roads connecting the towns, respectively. The towns are numbered from $1$ to $n$. 

In each of $m$ successive lines there are three integers separated by single spaces: $a, b$ and $l$, $a \neq b$. Each triple describes one one-way road of length $l$ enabling to move from the town $a$ to $b$. For each two towns there exist at most one road that enables to move in the given direction.

In the following line there is one integer $q$, denoting the number of queries. In the successive $q$ lines there are queries written, one per line. Each query has a form of three integers separated by single spaces: $c, d$ and $k$. Such a query refers to the length of the $k$-th shortest route from the town $c$ to the town $d$. 

�����ļ��ĵ�һ���������� $n,m$�����Ƿֱ��������������������ǵĵ�·�����������Ŵ� $1$ �� $n$��

������ $m$ �У�ÿ�� $3$ ��������$a,b$ �� $l$�����Ǵ���һ������Ϊ $l$ ����ߴ� $a$ �� $b$��������������������ͬ�������յ㡣

������һ����һ������ $q$������һ���� $q$ ��ѯ�ʡ������� $q$ ��ÿ����������$c,d$ �� $k$����ʾѯ�ʳ��� $c$ ������ $d$ �ĵ� $k$ ��·��

## �����ʽ

����ÿ��ѯ�ʣ����һ�б�ʾѯ��·���ĳ��ȣ�����𰸲����ڣ���� `-1`.

```input1
5 5
1 2 3
2 3 2
3 2 1
1 3 10
1 4 1
8
1 3 1
1 3 2
1 3 3
1 4 2
2 5 1
2 2 1
2 2 2
1 1 2
```

```output1
5
8
10
-1
-1
3
6
-1
```

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1 \le n \le 100$��$0 \le m \le n^2-n$��$1 \le l \le 500$��$1 \le q \le 10^4$��$1 \le k \le 100$��