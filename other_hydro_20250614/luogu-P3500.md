## ��Ŀ����
One of the tasks in the Byteotian Intelligence Test (BIT) is to cross out    numbers from an initial sequence in such a way that leaves as a result    certain given sequences.

Byteasar longs to become the IQ Master of Byteotia, but he is no good in    this kind of tasks.

But since practice makes perfect, he intends to practise a lot.

So much in fact that he asks you to write a program that will facilitate    the training by verifying his answers quickly.

## �����ʽ
The first line of the standard input contains one integer $m$ ($1\le m\le 1\ 000\ 000$).

The second line holds $m$ integers $a_1,a_2,\cdots,a_m$ ($1\le a_i\le 1\ 000\ 000$ for $1\le i\le m$), separated by single spaces,      that constitute the initial sequence of the test.

The third line of the input holds one integer $n$.

The following $2n$ lines describe the sequences to be obtained by crossing out      numbers from the initial sequence.

Each sequence's description takes two successive lines.

The first of these two lines contains an integer $m_i$ ($1\le m_i\le 1\ 000\ 000$).

The second contains an $m_i$-element long sequence of integers $b_{i,1},b_{i,2},\cdots,b_{i,m_i}$($1\le b_{i,j}\le 1\ 000\ 000$ for $1\le j\le m_i$)separated by single spaces. You may assume that the total length on given $n$ sequences does not exceed $1\ 000\ 000$.

## �����ʽ
Your program should print out $n$ lines to the standard output.

The $i$-th line (for $1\le i\le n$) should hold one word,      "TAK" (yes in Polish) if the $i$-th input sequence can be obtained by      crossing out (i.e., removing) some, not necessarily contiguous, numbers from the initial sequence,      or "NIE" (no in Polish) otherwise. Mind you, only the words should be printed,      no quotation marks. Of course, the order of the numbers left after crossing out is important,      as can be seen in the example.

## ��Ŀ����
### ��Ŀ����

**���� POI 2010 Stage 1.��[Intelligence Test](https://szkopul.edu.pl/problemset/problem/Arkza0f7GKKb-m1YZJulnlMk/site/?key=statement)��**

����һ��ĸ�� $a_1,a_2,a_3,\cdots ,a_n$ �����ɴ�ѯ�ʣ�ÿ��ѯ�ʸ���һ���Ӵ� $b_1,b_2,\cdots b_m$ �������������Ӵ��ǲ���ĸ���������С�

### �����ʽ

��һ��һ�������� $n$ ��  
�ڶ��� $n$ ���ո������������ $a_1,a_2,\cdots ,a_n$ ����ʾĸ����  
������һ�������� $q$ ����ʾѯ�ʴ�����  
������ $2 \times q$ �У�ÿ���б�ʾһ��ѯ�ʣ����еĵ�һ����һ�������� $m$ ���ڶ����� $m$ ���ո��������������ʾ $b_1,b_2,\cdots ,b_m$ ����ʾѯ�ʵ��Ӵ���

### �����ʽ

����� $q$ �У�ÿ��һ���ַ�����  
���� $i$ ��ѯ�ʵĴ���ĸ���������У���ô�� $i$ ��ӦΪ ```TAK``` ������ӦΪ ```NIE``` ��

���� $100\%$ �����ݣ��� $1\le n,m,a_i,b_i\le 1\ 000\ 000$ ���� $\sum m\le 1\ 000\ 000$ ������ $\sum m$ ��ʾ $q$ ��ѯ�ʵ� $m$ ֮�͡�

���������� [LibreOJ](https://loj.ac/p/2429)��

```input1
7
1 5 4 5 7 8 6
4
5
1 5 5 8 6
3
2 2 2
3
5 7 8
4
1 5 7 4
```

```output1
TAK
NIE
TAK
NIE
```

