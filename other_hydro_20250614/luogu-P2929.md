## ��Ŀ����
Farmer John has taken to yodeling from the top of the barn in order to communicate with the cows out in the pastures. Being bovine and all, cows can hear binary messages (0's and 1's) but have trouble with perfect communications because FJ's yodeling echoes off the silo. In fact, in a sequence of N (1 <= N <= 2,000) bits, Bessie will always receive a sequence of N bits, with the same number of 0s and 1s, but each 0 or 1 might be delayed.

Precisely speaking, for a given number D (0 <= D < N), the i-th bit might be heard as the j-th one as long as |i - j| <= D (in other words, no bit appears in a position farther than distance D from its original position). 
Consider the following message as an example: 0110. Four possible messages might be heard if D = 1: 0101, 0110, 1001, and 1010.

Given the message to be yodeled by FJ, along with two numbers D and K (1 <= K <= 100,000,000), determine the number of different messages that might be heard by Bessie, modulo 100,000,000. Also determine the K-th smallest such message in lexicographical order (in binary representation, with 0 coming before 1). It is guaranteed that K will be no larger than the number of different possible messages.

MEMORY LIMIT: 32 MB

TIME LIMIT: 2 seconds

FEEDBACK: Your first 50 submissions for this problem will be run on some of the official test data, and you will receive a summary of the results.

Լ�����ݶ��ϳ��裬�Դ�������ţ�ǽ�����������ţ�ǵ���������֣�����ֻ������Լ���ĸ������ $0$ �� $1$ ���ɵ���Ϣ��ʱ�����ӡ�Լ������������ $N  (1 \leq N \leq 2000)$ �� $0$ �� $1$����ţ������Ҳ�� $N$ �������� $0$ �� $1$ ����������仯������һ���� $0$ �� $1$ ����ƫ��ԭ����λ�ã������Լ���ĸ����ڴ���ʱ�����ġ������ӳ١�����$0$ �� $1$ ��ƫ����벻�ᳬ�� $D(O \leq D < N)$��Ҳ����˵ĳһ�����ԭ��λ�ú����ڵ�λ��֮��ľ���ֵ������ $D$��

���磬���� `0110`��$D = 1$�������ӳٷ�������ܳ��� `0101`��`0110`��`1001`��`1010` �����ִ���

����Լ�������� $01$ ����ʽ��һ������ $K(1 \leq K \leq10^8)$������㴫���ӳٷ�����һ���ж����ֿ��ܵ� $01$ �����Լ����е� $K$ ��Ĵ���ʲô��

## �����ʽ
\* Line 1: Three space-separated integers: N, D, and K

\* Line 2: FJ's binary message, containing exactly N bits


## �����ʽ
\* Line 1: The number of different possible messages that can heard by Bessie, mod 100,000,000

\* Line 2: The K-th smallest such message (in binary representation)

Note that if your program's first line of output is correct but the second line of output is either missing or wrong, you will receive 40% of the points for that test case.


```input1
4 1 3 
0110 

```

```output1
4 
1001 

```

