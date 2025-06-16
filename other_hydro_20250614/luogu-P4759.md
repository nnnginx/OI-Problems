## ��Ŀ����
Given an integer $N$, express it as the sum of at least two consecutive positive integers. For example:
   
   - $10 = 1 + 2 + 3 + 4$
   - $24 = 7 + 8 + 9$

If there are multiple solutions, output the one with the smallest possible number of summands.


## �����ʽ
The first line of input contains the number of test cases $T$. The descriptions of the test cases follow:

Each test case consists of one line containing an integer $N(1 \le N \le 10^9)$.

## �����ʽ
For each test case, output a single line containing the equation in the format:
``N = a + (a+1) + ... + b`` as in the example. If there is no solution, output a single word ``IMPOSSIBLE`` instead.


## ��Ŀ����
## ��Ŀ����

һ���� $T$ �����ݣ�ÿ�����ݸ���һ���� $N$���뽫 $N$ �ֽ�Ϊ���������������ĺͣ�����ж���������������С�����������

## �����ʽ��

��һ�У�һ������ $T$����ʾ����������

�� $2$ ������ $T+1$ �У�ÿ��һ������ $N$����ʾҪ��ֵ����֡�

## �����ʽ

 $T$ �У�ÿ��һ��ʽ�ӣ���ʾ��ֽ����

����޽⣬����� `IMPOSSIBLE`��


```input1
3
8
10
24

```

```output1
IMPOSSIBLE
10 = 1 + 2 + 3 + 4
24 = 7 + 8 + 9

```

