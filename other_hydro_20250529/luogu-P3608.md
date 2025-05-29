## ��Ŀ����
Farmer John is arranging his $N$ cows in a line to take a photo ($1 \leq N \leq 100,000$). The height of the $i$th cow in sequence is $h_i$, and the heights of all cows are distinct.

As with all photographs of his cows, FJ wants this one to come out looking as nice as possible. He decides that cow $i$ looks "unbalanced" if $L_i$ and $R_i$ differ by more than factor of 2, where $L_i$ and $R_i$ are the number of cows taller than $i$ on her left and right, respectively. That is, $i$ is unbalanced if the larger of $L_i$ and $R_i$ is strictly more than twice the smaller of these two numbers. FJ is hoping that not too many of his cows are unbalanced.

Please help FJ compute the total number of unbalanced cows.



## �����ʽ
The first line of input contains $N$.  The next $N$ lines contain $h_1 \ldots h_N$, each a nonnegative integer at most 1,000,000,000.



## �����ʽ
Please output a count of the number of cows that are unbalanced.



## ��Ŀ����
### ��Ŀ����

FJ ���ڰ������� $N$ ͷ��ţվ��һ�������գ�$1\le N \le 10^5$���������еĵ� $i$ ͷ��ţ�ĸ߶��� $h_i$�������������е���ţ����߶���ͬ��

������������ţ����Ƭһ����FJϣ��������Ƭ����ȥ�����ܺá�����Ϊ����� $L_i$ �� $R_i$ ����Ŀ��� $1$ �����ϣ��� $i$ ͷ��ţ���ǲ�ƽ��ģ�$L_i$ �� $R_i$ �ֱ����� $i$ ͷ��ţ�������߱����ߵ���ţ����������Ҳ����˵����� $L_i$ �� $R_i$ �еĽϴ������ڽ�С���� $2$ ������ $i$ ͷ��ţ���ǲ�ƽ��ġ�FJ ��ϣ������̫�����ţ��ƽ�⡣

����� FJ ���㲻ƽ�����ţ������

### �����ʽ

��һ��һ������ $N$��

���� $N$ �а��� $H_1$ �� $H_n$��ÿ��һ�������� $10^9$ �ķǸ�������

### �����ʽ

�������ƽ�����ţ������

```input1
7
34
6
23
0
5
99
2
```

```output1
3
```

