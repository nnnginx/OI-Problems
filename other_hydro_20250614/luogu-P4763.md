## ��Ŀ����
You are given a sequence of white $(W)$ and black $(B)$ bricks. The goal is to partition it into some number of non-empty, contiguous blocks, each one having the same ratio of white and black bricks.

Of course one can always ��partition�� the sequence into one single block (which is not very interesting). We want, however, to have as many blocks as possible. Consider for example the following sequences and its partitions:

   - $BWWWBB = BW + WWBB$ (ratio 1:1),
   - $WWWBBBWWWWWWWWWB = WWWB + BBWWWWWW + WWWB$ (ratio 3:1).

Note that both of these partitions are optimal with respect to the number of blocks.


## �����ʽ
The first line of input contains the number of test cases $T$. The descriptions of the test cases follow:

Each test case starts with one line containing an integer $n(1 \le n \le 10^5)$ which is the length of the description of a sequence. Each of the following $n$ lines consists of an integer $k(1 \le k \le 10^9)$ and one of the characters $W$ or $B$, meaning that $k$ bricks of the given color follow next in the sequence. It is guaranteed that the total length of the brick sequence does not exceed $10^9$.

## �����ʽ
For each test case, output a single line containing the largest possible number of blocks.


## ��Ŀ����
��Ŀ����  
����һ����'B'��'W'��ɵ����У����䰴�ֳ�����������ÿ�������'B':'W'��ֵ���  

���������ʽ  

�����ʽ��  
�������ݣ���һ��һ������T��ʾ��������  
ÿ�����ݵĵ�һ��Ϊһ������n��������n�У�ÿ��һ������k��һ���ַ���'B'��'W'����ʾ����һ�����к���һ������Ϊk��'B'��'W'�����У����е��ܳ��Ȳ�����10^9  

�����ʽ��
��T�У�ÿ��һ��������ʾ�ֳܷɵ�����������  

```input1
3
3
1 B
3 W
2 B
4
3 W
3 B
9 W
1 B
2
2 W
3 W
```

```output1
2
3
5
```

