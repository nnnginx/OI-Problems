## ��Ŀ����
Following up on a journal article about increasing milk production, Bessie has become the Baric Bovine by studying atmospheric pressure in order to curry favor with Farmer John.

She takes N (1 <= N <= 100) measurements conveniently named M\_1 through M\_N during the day (1 <= M\_i <= 1,000,000); these measurements are numbered in the order in which Bessie observed them.

In order to characterize the day's atmospheric pressure readings, she is interested in finding a subset of the measurements (given by the K (1 <= K <= N) indices s\_j where 1 <= s\_1 < s\_2 < ... < s\_K <= N) that accurately reflects the entire set, i.e., limits the error as described below.

In any subset of measurements, an error is incurred for each

measurement (1) before the first member of the subset, (2) between two consecutive measurements in the subset, and (3) after the last member of the subset. The total error value for a given set of s\_j values is the sum of each of the individual errors.

Specifically, for all measurements whose index i is not one of the s\_j values:

```cpp
* if i is less than s_1, then the sample error is: 
2 * | M_i - M_(s_1) | 
* if i is between s_j and s_(j+1), then the sample error is 
| 2 * M_i - Sum(s_j, s_(j+1)) | 
where Sum(x, y) = M_x + M_y; 
* if i is greater than s_K, then the sample error is 
2 * | M_i - M_(s_K) | 
Given a maximum error value E (1 <= E <= 1,000,000), determine the size of the smallest subset of measurements that produces an error of at most E. 
```


## �����ʽ
\* Line 1: Two space-separated integers: N and E

\* Lines 2..N+1: Line i+1 contains a single integer: M\_i


## �����ʽ
\* Line 1: Two space-separated integers: the size of the smallest subset of measurements that produces an error of at most E and the least possible error for the subset of that size.


## ��Ŀ����
## ��Ŀ����

Ϊ���о�ũ��������Bessie ����ũ�� John ����  $N$ ����ѹ��������˳���¼�˽��  $M_1 \cdots M_n$��Bessie ���ҳ�һ���ֲ���������ܽ�һ�������ѹ�ֲ���������  $K(1 \leq K \leq N)$ ����  $s_j (1 \leq s_1 < s_2 < \cdots < s_K \leq N)$ ���������в�������������������µ����: �����κβ�������Ӽ���ÿһ���Ǵ��Ӽ��еĽ���������������������в�����������֮�͡�����ȷ��˵������ÿһ��������  $s_j$ ����ͬ��  $i$��

- ���  $i$ С��  $s_1$, ����ǣ� $2 \times | M_i - M_{(s_1)} |$��
- ���  $i$ ��  $s_j$ ��  $s_{(j+1)}$ ֮�䣬����ǣ� $| 2 \times M_i - \operatorname{Sum}(s_j, s_{(j+1)}) |$��ע�� $\operatorname{Sum}(x, y) = M_x + M_y$  ( $M_x$ ��  $M_y$ ֮��)��
- ���  $i$ ����  $s_K$ ,���Ϊ�� $2 \times | M_i - M_{(s_K)} |$ ���������������  $E$���ҳ���С��һ���ֽ��ʹ��������Ϊ  $E$��

## �����ʽ

- ��  $1$ �У������ÿո�ֿ���������  $N$ ��  $E$��

- ��  $2\cdots N+1$ �У���  $i+1$ �а���������һ��������  $M_i$��

## �����ʽ

- ��  $1$ �У������ÿո�ֿ����������ֱ��������С��ʹ�����С�ڵ���  $E$ �Ĳ�������Ӽ�Ԫ�ص����������ܴﵽ����С���ֵ��

## ˵��/��ʾ

### ���ݷ�Χ

�����������ݣ� $1 \leq N \leq 100$�� $1 \leq M_i \leq 1,000,000$�� $1 \leq E \leq 1,000,000$��

### ����˵��

Bessie ���� 4 �β������������������ 20�������Ľ���ֱ�Ϊ 10��3��20 �� 40��

ѡ��ڶ��κ͵��Ĵβ����������ѵģ����Ϊ 17����һ����������Ϊ  $2\times|10-3|=14$����������Ϊ  $|2\times20-(3+40)|=3$��

```input1
4 20 
10 
3 
20 
40 

```

```output1
2 17 

```

## ��ʾ
Bessie takes four measurements; the maximum error is 20. The

measurements are, in sequence: 10, 3, 20, and 40.


Choosing the second and fourth measurements is the best option, giving an error of 17. The first term's error is 2\*|10-3| = 14; the third term's error is |2\*20 - (3+40)| = 3. 

