## ��Ŀ����


There are $n$ crates waiting to be loaded onto a ship. The crates are numbered $1 , 2 , \cdots , n$ , the numbers determining the order of loading. Unfortunately, someone messed up the transit and the crates are standing in a row in an arbitrary order. As there is only limited space in the dock area, you must sort the crates by swapping some of them.

You are given a crane that works in the following way: you select a connected interval of crates of even length. The crane then exchanges the first half of the interval with the second half. The order inside both halves remains unchanged. Determine the sequence of crane moves that reorders the crates properly.

The crane's software has a bug: the move counter is a $9-based$ (not $10-based,$ as you might think) integer with at most $6$ digits. Therefore, the crane stops working (and has to be serviced) after $9^{6} = 531441$ moves. Your solution must fit within this limit.



## �����ʽ


The first line of input contains the number of test cases $T$ . The descriptions of the test cases follow:

Each test case starts with an integer $n , 1 \le n \le 10 000$ , denoting the number of crates. In the next line a permutation of numbers ${1 , 2 , \cdots $ , n} follows.



## �����ʽ


For each test case print a single line containing $m -$ the number of swaps $-$ followed by $m$ lines describing the swaps in the order in which they should be performed. A single swap is described by two numbers $-$ the indices of the first and the last element in the interval to be exchanged. Do not follow the crane's strange software design $-$ use standard decimal numeral system.



## ��Ŀ����
�� $n$ �����ӵ���װ�ϴ������ӵı���� $a_1,a_2,\cdots,a_n$����Ĺ�����ͨ�����ɴν����������Ǵ�С�������С���ÿ�ο���ѡ��һ�����䣬������ǰ�벿�����벿�ֽ����������ڲ���˳�򱣳ֲ��䡣�������Խ��� $531441$ �Ρ� 

### �����ʽ

��һ����������������� $T$��

������ $2\times T$ �У���ʾ $T$ �����ݡ�ÿ�����ݵĵ�һ��Ϊ $n\ (1 \leq n \leq 10000)$����ʾ���ӵ��������ڶ���Ϊ $n$ ��������$a_1,a_2,\cdots,a_n $ ����ʾ���ӵı�š�

### �����ʽ

����ÿ�����ݣ��������һ���� $m$ ����ʾ�����Ĵ����� Ȼ����� $m$ �У�����˳������ÿһ�ν���������ÿ�ν��������Ҫ�����������е�һ��Ԫ�غ����һ��Ԫ�ص��±ꡣ

```input1
2
6
5 4 6 3 2 1
5
1 2 3 4 5

```

```output1
5
1 2
4 5
5 6
4 5
1 6
0

```

## ��ʾ
Time limit: 4 s, Memory limit: 128 MB. 



