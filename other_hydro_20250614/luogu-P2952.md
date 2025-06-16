## ��Ŀ����
Farmer John's N cows (conveniently numbered 1..N) are forming a line. The line begins with no cows and then, as time progresses, one by one, the cows join the line on the left or right side. Every once in a while, some number of cows on the left or right side of the line all leave the line to go graze in their favorite pasture.

FJ has trouble keeping track of all the cows in the line. Please help him.

The cows enter the line in numerical order 1..N, and once a cow leaves the line she never re-enters it. Your program will be given S (1 <= S <= 100,000) input specifications; each appears on a single line and is one of two types:

\* A cow enters the line (a parameter indicates whether on the left or right).

\* K cows leave the line from the left or right side (supplied parameters define both the number of cows and which side).

Input lines never request an operation that can not be performed.

After all the input lines have been processed, your program should print the cows in the line in order from left to right. The final line is guaranteed to be non-empty at the end of the input specifications.

## �����ʽ
\* Line 1: A single integer: S

\* Lines 2..S+1: Line i+1 contains specification i in one of four formats:

\* A L -- a cow arrives on the Left of the line

\* A R -- a cow arrives on the Right of the line

\* D L K -- K cows depart the Left side of the line

\* D R K -- K cows depart the Right side of the line

## �����ʽ
\* Lines 1..??: Print the numbers of the cows in the line in order from left to right, one number per line.

## ��Ŀ����
Farmer John�����¼�� FJ���� $N$ ͷ��ţ���� $1 \dots N$ ��ţ���ֱ�����Ŷӡ�һ��ʼ����������û���κ���ţ������ʱ������ƣ���ţ�ǻ�һ����һ����վ���������߻��ұߡ��ֹ���һ�����ĳЩ��ţ��Ӷ������뿪��ȥ���Լ���ϲ���Ĳ��ϡ�

FJ �޷�����ÿһͷ��ţ�����ǣ�������������������

��ţ�� $1 \dots N$ ��˳���Ŷӣ������뿪����ţ�����ٴλ��������ݽ������ $S$��$1 \le S \le 100000$�� ��ָ���ռһ�У������֣�

- $A$ ͷ��ţ�����˶��У�����һ����������ʾ������뻹�Ǵ��Ҽ��룩��
- $K$ ͷ��ţ����߻����ұ��뿪�˶��У����������������ֱ��ʾ�����뿪���Ǵ����뿪���뿪����ͷ��ţ����

���������һ���ǿ���ִ�еġ�

���еĲ�����������ĳ���Ӧ���Դ����ҵ�˳����������ţ���С����ݱ�֤���Ķ��в��ա�

**�������ʽ��**

- �� $1$ �У�����һ������ $S$��
- �� $2 \dots S+1$ �У��� $i+1$ �л���һ����������¼��֣�
  - `A L`��һͷ��ţ�Ӷ�����߼��룻
  - `A R`��һͷ��ţ�Ӷ����ұ߼��룻
  - `D L K`��$K$ ͷ��ţ�Ӷ�������뿪��
  - `D R K`��$K$ ͷ��ţ�Ӷ����ұ��뿪��

**�������ʽ��**

- �� $1 \dots ??$ �У����������������ţ���У�һ����ţ���ռһ�С�

**���������͡�**

����Ϊ����������Ӧ�Ķ��У�

- `A L`��$1$��
- `A L`��$2,1$��
- `A R`��$2,1,3$��
- `A L`��$4,2,1,3$��
- `D R 2`��$4,2$��
- `A R`��$4,2,5$��
- `A R`��$4,2,5,6$��
- `D L 1`��$2,5,6$��
- `A L`��$7,2,5,6$��
- `A R`���������У���$7,2,5,6,8$��

```input1
10 
A L 
A L 
A R 
A L 
D R 2 
A R 
A R 
D L 1 
A L 
A R 

```

```output1
7 
2 
5 
6 
8 

```

## ��ʾ
Input    Resulting Cow Line

A L      1

A L      2 1

A R      2 1 3

A L      4 2 1 3

D R 2    4 2

A R      4 2 5

A R      4 2 5 6

D L 1    2 5 6

A L      7 2 5 6

A R      7 2 5 6 8

��л@ ws\_fuweidong  �ṩ���롣


