## ��Ŀ����
Farmer John is trying to hire contractors to help rearrange his farm, but so far all of them have quit when they saw the complicated sequence of instructions FJ wanted them to follow.  Left to complete the project by himself, he realizes that indeed, he has made the project perhaps more  complicated than necessary.  Please help him follow his instructions to  complete the farm upgrade.

FJ's farm consists of $N$ fields in a row, conveniently numbered $1 \ldots N$. In each field there can be any number of haybales.  Farmer John's instructions contain three types of entries:

1) Given a contiguous interval of fields, add a new haybale to each field.

2) Given a contiguous interval of fields, determine the minimum number of haybales in a field within that interval.

3) Given a contiguous interval of fields, count the total number of haybales  inside that interval.

## �����ʽ
The first line contains two positive integers, $N$ ($1 \leq N \leq 200,000$) and $Q$ ($1 \leq Q \leq 100,000$).

The next line contains $N$ nonnegative integers, each at most 100,000, indicating how many haybales are initially in each field.

Each of the next $Q$ lines contains a single uppercase letter, either M, P or S, followed by either two positive integers $A$ and $B$ ($1 \leq A \leq B \leq N$), or three positive integers $A$, $B$, and $C$ ($1 \leq A \leq B \leq N$; $1 \leq C \leq 100,000$).  There will be three positive integers if and only if the uppercase letter is P.

If the letter is M, print the minimum number of haybales in the interval of fields from $A \ldots B$.

If the letter is P, put $C$ new haybales in each field in the interval of fields from $A \ldots B$.

If the letter is S, print the total number of haybales found within interval of fields from $A \ldots B$.

## �����ʽ
A line in the output should appear in response to every 'M' or 'S' entry in FJ's instructions.

## ��Ŀ����
### ��Ŀ����

Farmer John ���ڳ��Թ�Ӷ�а��������������°���ũ��������ĿǰΪֹ�����га����ڿ��� FJ ϣ��������ѭ�ĸ���ָ�����к󶼴�ְ�ˡ�FJ ���ò��Լ���������Ŀ������ʶ���Լ����ܰ���Ŀ��ñȱ�Ҫ�Ļ�Ҫ���ӡ������������ָ�����ũ����������

FJ ��ũ����һ�� $N$ �������ɣ����Ϊ $1 \ldots N$��ÿ���������������������ĸɲݶѡ�Farmer John ��ָ������������͵���Ŀ��

1) ����һ��������������䣬��ÿ��������һ���µĸɲݶѡ�

2) ����һ��������������䣬ȷ��������������иɲݶѵ���С������

3) ����һ��������������䣬����������ڸɲݶѵ�������

### �����ʽ

��һ�а���������������$N$��$1 \leq N \leq 200,000$���� $Q$��$1 \leq Q \leq 100,000$����

�ڶ��а��� $N$ ���Ǹ�������ÿ���������Ϊ $100,000$����ʾÿ������г�ʼ�ĸɲݶ�������

�������� $Q$ ��ÿ�а���һ����д��ĸ�������� M��P �� S��������������� $A$ �� $B$��$1 \leq A \leq B \leq N$������������������ $A$��$B$ �� $C$��$1 \leq A \leq B \leq N$��$1 \leq C \leq 100,000$����ֻ�е���д��ĸ�� P ʱ���Ż���������������

�����ĸ�� M������� $A \ldots B$ ����������ڸɲݶѵ���С������

�����ĸ�� P����� $A \ldots B$ ����������ڵ�ÿ�������� $C$ ���µĸɲݶѡ�

�����ĸ�� S������� $A \ldots B$ ����������ڸɲݶѵ�������

### �����ʽ

���� FJ ָ���е�ÿһ�� 'M' �� 'S' ��Ŀ�����һ����Ӧ�Ľ����

```input1
4 5
3 1 2 4
M 3 4
S 1 3
P 2 3 1
M 3 4
S 1 3
```

```output1
2
6
3
8
```

