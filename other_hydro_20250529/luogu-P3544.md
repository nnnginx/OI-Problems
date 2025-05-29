## ��Ŀ����
A map of Mafiatown's road network is given.

The network consists of intersections and bidirectional streets that connect them.

The streets cross only at the intersections, but they may lead through tunnels or flyovers.

Each pair of intersections is linked by at most one street.

At every intersection $v$ there is a police station manned by $p(v)$ policemen.

A street linking the intersections $u$ and $v$ is considered safe if there are at least $b(u,v)$ policemen in total in the two stations at the streets ends. Initially    $p(u)+p(v)\ge b(u,v)$ holds for every street.

However, due to an ongoing crisis the mayor Byteasar has ordained the Minimalist Security Act (MSA), which states that:

a certain number (which may be zero) of policemen is to be laid off from each police station        (we denote the number of policemen laid off from the station at the intersection $v$ by $z(v)$),                  after the layoff, the total number of the policemen at both ends of every street connecting some two intersections,        say $u$ and $v$, should equal $b(u,v)$ exactly, i.e.:

$p(u)-z(u)+p(v)-z(v)=b(u,v)$ These rules do not determine uniquely how many policemen are to be laid off.

Byteasar wonders what is the minimum and the maximum number of laid off policemen    (the sum of $z$ values over all intersections) that complies with aforementioned rules.

## �����ʽ
In the first line of the standard input there are two integers, $n$ and $m$ ($1\le n\le 500\ 000$, $0\le m\le 3\ 000\ 000$), separated by a single space, that denote    the number of intersections and the number of streets in Mafiatown, respectively.

The intersections are numbered from 1 to $n$.

In the second line $n$ nonnegative integers separated by single spaces are given.

These are the numbers of policemen currently employed at successive stations, i.e., the values $p(1),p(2),\cdots,p(n)$($0\le p(i)\le 10^6$).

Each of the following $m$ lines describes a single bidirectional street. Such description consists of three integers,$u_i,v_i,b(u_i,v_i)$($1\le u_i,v_i\le n$,$u_i\ne v_i$,$0\le b(u_i,v_i)\le 10^6$), separated by single spaces, that denote respectively: the numbers of the intersections at the ends of the street and the minimum total number of policemen that have to man the stations at those intersections.


## �����ʽ
If Byteasar's ordinance can be carried out, your program should print, on the standard output,    exactly one line with two integers separated by a single space.

The numbers should be the minimum and the maximum number of policemen that should be laid off    in order to carry out the ordinance.

If carrying out the ordinance is impossible, your program should print a single line containing    the word NIE (Polish for no).


## ��Ŀ����
### ��Ŀ����

**���� POI 2012 Stage 3. Day 2��[Bezpiecze��stwo minimalistyczne](https://szkopul.edu.pl/problemset/problem/aSbIC_LB4H-CGMYPEVue5jFw/site/?key=statement)��**

����һ������ͼ�����е�Ȩ $p(v)$�����б�Ȩ $b(u,v)$����ʼʱ��֤��ÿ������ $p(u) + p(v) \ge b(u,v)$��

������Ҫ����һ���ֵ�ĵ�Ȩ��ʹ�ö�ÿ���߶�ǡ�� $p(u) + p(v) = b(u,v)$.

������ͼ���ٵĵ�Ȩ�͵���Сֵ�����ֵ��

### �����ʽ

��һ���������� $n$ �� $m$��$1 \le n \le 500\ 000,0 \le m \le 3\ 000\ 000$������ʾͼ�ĵ����ͱ�����

������һ�� $n$ ���Ǹ����� $p(1),p(2),\ldots,p(n) (0 \le p(i) \le 10^6)$����ʾ��Ȩ��

������ $m$ ��ÿ���������� $u_i, v_i, b(u_i, v_i)$��$1 \le u_i,v_i \le n,u_i \neq v_i,0 \le b(u_i,v_i) \le 10^6$������ʾ�ߺͱ�Ȩ��

### �����ʽ

������ڷ��������ķ��������һ��������������ʾ����ͼ���ٵĵ�Ȩ�͵���Сֵ�����ֵ��

��������ڣ���� `NIE`.

### ���ݷ�Χ

���� $56\%$ �������� $n \le 2000,m \le 8000$.

�������������� $1 \le n \le 500\ 000,0 \le m \le 3\ 000\ 000$.

���������� [LibreOJ](https://loj.ac/p/2702)��

```input1
3 2
5 10 5
1 2 5
2 3 3
```

```output1
12 15
```

