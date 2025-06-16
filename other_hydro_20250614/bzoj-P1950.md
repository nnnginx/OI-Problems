## ��Ŀ����

Webmaster Kirk is reorganizing his school's website. There are a number of pages on the website and the content is fine, but he noticed that the pages are not properly linked. In fact, every page contains exactly one link, pointing to some other page in the website. This is a poor design �C starting from the homepage, a visitor will usually have to follow many links before reaching the page of his interest, and some pages might not be reachable from the homepage at all. As a first step, he wants to add a few links so that every page can be quickly accessed from the homepage. New links can be added anywhere in the website.

The website contains $n$ pages marked with integers $1$ to $n$ and the homepage is marked with the number $1$.

There are also $n$ links; each page contains exactly one link pointing to some different page. For an integer $k$, a website is said to be $k$-reachable if every page on the website other than the homepage can be reached from the homepage by following at most $k$ links.

Write a program that, given the description of the website and an integer $k$, finds the minimum number of links that need to be added in order to make the website $k$-reachable.

���� $n$ ���� $n$ ���ߵ�����ͼ��Ҫ������С�ıߣ�ʹ�õ� $1$ �����������е�����·���Ȳ����� $k$��

## �����ʽ

The first line of input contains two integers $n$ and $k$ �C the number of pages and the target maximum number of links to be followed. Each of the following $n$ lines contains two different integers $a$ and $b$ ($b \le a$, $b \le n$) meaning that the link on page $a$ points to page $b$.

## �����ʽ

The first and only line of output should contain a single integer, the minimum number of additional links required to make the website $k$-reachable.

```input1
14 4
1 2
2 3
3 4
4 5
7 5
5 6
6 3
8 10
10 9
9 8
14 13
13 12
12 11
11 14
```

```output1
3
```

## ����˵�� 1

One possible solution is to add the links $1 \to 7$, $1 \to 14$ and $14 \to 10$.

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$2 \le n \le 5 \times 10^5$��$1 \le k \le 2 \times 10^4$��