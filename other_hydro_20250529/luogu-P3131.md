## ��Ŀ����
Farmer John's $N$ cows are standing in a row, as they have a tendency to do from time to time.  Each cow is labeled with a distinct integer ID number so FJ can tell them apart. FJ would like to take a photo of a contiguous group of cows but, due to a traumatic  childhood incident involving the numbers $1 \ldots 6$, he only wants to take a picture of a group of cows if their IDs add up to a multiple of 7.

Please help FJ determine the size of the largest group he can photograph.

## �����ʽ
The first line of input contains $N$ ($1 \leq N \leq 50,000$).  The next $N$ lines each contain the $N$ integer IDs of the cows (all are in the range $0 \ldots 1,000,000$).


## �����ʽ
Please output the number of cows in the largest consecutive group whose IDs sum to a multiple of 7. If no such group exists, output 0.

## ��Ŀ����
### ��Ŀ����

Farmer John �� $N$ ͷ��ţվ��һ�ţ���������ʱ��ʱ���������顣ÿͷ��ţ����һ�����ص����� ID ��ţ��Ա� Farmer John �ܹ��������ǡ�Farmer John ϣ��Ϊһ����������ţ���գ�������ͯ��ʱ������ $1 \ldots 6$ ��صĴ����¼�����ֻϣ������һ����ţ��������ǵ� ID �������� 7 �ı�����

����� Farmer John ȷ������������������ţ��Ĵ�С��

### �����ʽ

����ĵ�һ�а��� $N$��$1 \leq N \leq 50,000$������������ $N$ ��ÿ�а���һͷ��ţ������ ID������ ID ���� $0 \ldots 1,000,000$ ��Χ�ڣ���

### �����ʽ

����� ID ֮��Ϊ 7 �ı��������������ţ���е���ţ����������������������飬����� 0��

### ˵��/��ʾ

����������У�$5+1+6+2+14 = 28$��

```input1
7
3
5
1
6
2
14
10
```

```output1
5
```

## ��ʾ
In this example, $5+1+6+2+14 = 28$.

