## ��Ŀ����
Each of Farmer John's N (4 <= N <= 16) cows has a unique serial number S\_i (1 <= S\_i <= 25,000). The cows are so proud of it that each one now wears her number in a gangsta manner engraved in large letters on a gold plate hung around her ample bovine neck.

Gangsta cows are rebellious and line up to be milked in an order called 'Mixed Up'. A cow order is 'Mixed Up' if the sequence of serial numbers formed by their milking line is such that the serial numbers of every pair of consecutive cows in line differs by more than K (1 <= K <= 3400). For example, if N = 6 and K = 1 then 1, 3, 5, 2, 6, 4 is a 'Mixed Up' lineup but 1, 3, 6, 5, 2, 4 is not (since the consecutive numbers 5 and 6 differ by 1).

How many different ways can N cows be Mixed Up?

For your first 10 submissions, you will be provided with the results of running your program on a part of the actual test data.

POINTS: 200

Լ������Nͷ��ţ����iͷ��ţ�ı����Si��ÿͷ��ţ�ı�Ŷ���Ψһ�ġ���Щ��ţ��� ����Ƣ����Ϊ��ﲻ���������������ڼ��̵�ʱ��һ��Ҫ�ųɻ��ҵĶ��顣��һֻ���ҵĶ� ���У�������ţ�ı��֮�������K�����統K = 1ʱ��1, 3, 5, 2, 6, 4����һ֧���ҵĶ��飬 ��1, 3, 6, 5, 2, 4���ǣ���Ϊ6��5ֻ��1������һ�����ж����ֶ����ǻ��ҵ��أ�


## �����ʽ
\* Line 1: Two space-separated integers: N and K

\* Lines 2..N+1: Line i+1 contains a single integer that is the serial number of cow i: S\_i


## �����ʽ
\* Line 1: A single integer that is the number of ways that N cows can be 'Mixed Up'. The answer is guaranteed to fit in a 64 bit integer.


```input1
4 1 
3 
4 
2 
1 

```

```output1
2 

```

## ��ʾ
The 2 possible Mixed Up arrangements are:

3 1 4 2

2 4 1 3


