## ��Ŀ����
�������ݼ�������ʱ������Ҫ�ϳ�ʱ��ȴ���

## ��Ŀ����
```plain
Byteasar intends to throw up a party.
```
Naturally, he would like it to be a success.  Furthermore, Byteasar is quite certain that to make it so it suffices if all invited guests  know each other.  He is currently trying to come up with a list of his friends he would like to invite.

Byteasar has $n$ friends, where $n$ is divisible by 3.

```plain
Fortunately, most of Byteasar's friends know one another.
```
Furthermore, Byteasar recalls that he once attended a party where there were $\frac{2}{3}n$ of his friends, and where everyone knew everyone else.

Unfortunately, Byteasar does not quite remember anything else from that    party.


In particular, he has no idea which of his friends attended it.

Byteasar does not feel obliged to throw a huge party, but he would like to    invite at least \frac{n}{3} of his friends.



He has no idea how to choose them, so he asks you for help.

## �����ʽ
In the first line of the standard input two integers, $n$ and $m$ ($3\le n\le 3\ 000$, $\frac{\frac{2}{3}n(\frac{2}{3}n-1)}{2}\leq m\leq \frac{n(n-1)}{2}$), are given,separated by a single space.  These denote the number of Byteasar's friends and the number of pairs of his friends who know each other, respectively.

Byteasar's friends are numbered from 1 to $n$.

Each of the following $m$ lines holds two integers separated by a single      space.

The numbers in line no. $i+1$ (for $i=1,2,...,m$) are $a_i$ and $b_i$($1\le a_i<b_i\le n$), separated by a single space, which denote that the persons $a_i$ and $b_i$ know each other. Every pair of numbers appears at most once on the input.


## �����ʽ
In the first and only line of the standard output your program should      print $\frac{n}{3}$ numbers, separated by single spaces, in increasing      order.  These number should specify the numbers of Byteasar's friends whom      he should invite to the party.  As there are multiple solutions, pick one      arbitrarily.


## ��Ŀ����
### ��Ŀ����

**���� POI 2011 Round 3. Day 1. A��[Party](https://szkopul.edu.pl/problemset/problem/PCtteC6gKwc2ZikW8nUZzfyh/site/?key=statement)��**

Byteasar �������һ�ξۻᡣ����Ȼ��Ҫ��ξۻ�ɹ����С����⣬Byteasar ȷ��ֻҪ����ļα���������ʶ�Ϳ����ˡ���Ŀǰ������дһ������������

Byteasar �� $n$ �����ѣ����� $n$ ���Ա� $3$ ���������˵��ǣ�Byteasar �����Ѵ󲿷ֶ�������ʶ������ Byteasar ������һ�����μӵľۻᣬ�Ǵξۻ��� $ \frac{2}{3}n $ ���������Ѳμӣ��������Ƕ�������ʶ�����ҵ��ǣ������Ǵξۻ�ľ���ϸ�������ǵ��ˡ����ܵ���˵����������������Щ���Ѳμ��ˡ�

Byteasar ��Ϊ��û������ٰ�һ�����;ۻᣬ�������������� $ \frac{n}{3} $ ���������ѡ�����֪������˭���������������

### �����ʽ

����ĵ�һ�а����������� $n,m$����ʾ Byteasar ���������ͻ�����ʶ�����Ѷ�����

������ $m$ �У�ÿ���������� $a_i,b_i$�� ��ʾ���� $a_i,b_i$ ������ʶ��ÿһ��������������г���һ�Ρ�

### �����ʽ

������������һ�� $ \frac{n}{3} $ ��������ʾ Byteasar Ҫ��������ѱ�š�����ж���⣬�������һ����ɡ�

### ��������

![](https://cdn.luogu.com.cn/upload/image_hosting/yjpf686v.png)

���Ϊ $1,3,4,5$ �����ѻ�����ʶ��Ȼ����������һ�Ի�����ʶ�����ѣ��� $2,4$����������Ϊ��ȷ�𰸡�������һ�����Ѳ���һ��������֮ǰ�ᵽ���Ǹ���Ԫ�顣

### ���ݷ�Χ

����ȫ�����ݣ�$ 3 \le n \le 3000 , \frac{\frac{2}{3}n(\frac{2}{3}n-1)}{2} \le m \le \frac{n(n-1)}{2}, 1 \le a_i \lt b_i \le n $��

���������� [LibreOJ](https://loj.ac/p/2166)��

```input1
6 10
2 5
1 4
1 5
2 4
1 3
4 5
4 6
3 5
3 4
3 6
```

```output1
2 4
```

