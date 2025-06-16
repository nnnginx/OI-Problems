## ��Ŀ����
Bessie the cow was excited to recently return to in-person learning! Unfortunately, her instructor, Farmer John, is a very boring lecturer, and so she ends up falling asleep in class often.
Farmer John has noticed that Bessie has not been paying attention in class. He has asked another student in class, Elsie, to keep track of the number of times Bessie falls asleep in a given class. There are $N$ class periods $(1\le N\le 10^5)$, and Elsie logs that Bessie fell asleep $a_i$ times $(0\le a_i\le 10^6)$ in the $i$-th class period. The total number of times Bessie fell asleep across all class periods is at most $10^6$.

Elsie, feeling very competitive with Bessie, wants to make Farmer John feel like Bessie is consistently falling asleep the same number of times in every class -- making it appear that the issue is entirely Bessie's fault, with no dependence on Farmer John's sometimes-boring lectures. The only way Elsie may modify the log is by combining two adjacent class periods. For example, if $a=[1,2,3,4,5]$, then if Elsie combines the second and third class periods the log will become $[1,5,4,5]$.

Help Elsie compute the minimum number of modifications to the log that she needs to make so that she can make all the numbers in the log equal.

## �����ʽ
Each input will contain $T$ $(1\le T\le 10)$ test cases that should be solved independently.

The first line contains $T$, the number of test cases to be solved. The $T$ test cases follow, each described by a pair of lines. The first line of each pair contains $N$, and the second contains $a_1,a_2,\ldots,a_N$. 

It is guaranteed that within each test case, the sum of all values in $a$ is at most $10^6$. It is also guaranteed that the sum of $N$ over all test cases is at most $10^5$.

## �����ʽ
Please write $T$ lines of output, giving the minimum number of modifications Elsie could perform to make all the log entries equal for each case.

## ��Ŀ����
### ��Ŀ����

��ţ Bessie ����ܸ����ܹ��ط����¿��ã����ҵ��ǣ�������ʦ Farmer John ���ηǳ����ģ�����������ڿ�����˯�š�  
Farmer John ע�⵽ Bessie �ڿ�����û��ר�����������ð��ϵ���һλѧ�� Elsie ��¼ Bessie ��ÿ�ڿ���˯�ŵĴ������ܹ��� $N$ �ڿΣ�$1 \leq N \leq 10^5$����Elsie ��¼�� Bessie �ڵ� $i$ �ڿ���˯���� $a_i$ �Σ�$0 \leq a_i \leq 10^6$�������пγ��� Bessie ˯�ŵ��ܴ��������� $10^6$��

Elsie �� Bessie �е��ǳ���������ϣ���� Farmer John ���� Bessie ��ÿ�ڿ���˯�ŵĴ�����һ�µġ��������⿴������ȫ�� Bessie �Ĵ����� Farmer John ��ʱ���ĵĽ����޹ء�Elsie �޸ļ�¼��Ψһ��ʽ�ǽ��������ڵĿκϲ������磬��� $a = [1,2,3,4,5]$����ô��� Elsie �ϲ��ڶ��͵����ڿΣ���¼����Ϊ $[1,5,4,5]$��

����� Elsie ��������Ҫ�Լ�¼���е������޸Ĵ�������ʹ��¼�е�����������ȡ�

### �����ʽ

ÿ��������� $T$��$1 \leq T \leq 10$������Ҫ��������Ĳ���������

��һ�а��� $T$����ʾ������������������������ $T$ �����������ÿ��������������ÿ��ĵ�һ�а��� $N$���ڶ��а��� $a_1, a_2, \ldots, a_N$��

��֤ÿ�����������У�$a$ ������ֵ֮�Ͳ����� $10^6$��ͬʱ�����в��������� $N$ ֮�Ͳ����� $10^5$��

### �����ʽ

����� $T$ �У�ÿ�б�ʾ Elsie Ϊʹ��¼�е����������������������޸Ĵ�����

### ��ʾ

���ڵ�һ������������Elsie ����ͨ�� 3 ���޸Ľ���¼��ΪȫΪ $3$��
```
   1 2 3 1 1 1
-> 3 3 1 1 1
-> 3 3 2 1
-> 3 3 3
```

���ڵڶ�������������Elsie ����ͨ�� 2 ���޸Ľ���¼��ΪȫΪ $7$��
```
   2 2 3
-> 2 5
-> 7
```

�������һ������������Elsie ����Ҫ�����κβ�������Ϊ��¼�Ѿ�����ͬ��������ɡ�

```input1
3
6
1 2 3 1 1 1
3
2 2 3
5
0 0 0 0 0
```

```output1
3
2
0
```

## ��ʾ
���������͡�

For the first test case in this example, Elsie can change her log to consist solely of 3s with 3 modifications.
```
   1 2 3 1 1 1
-> 3 3 1 1 1
-> 3 3 2 1
-> 3 3 3
```
For the second test case, Elsie can change her log to 7 with 2 modifications.
```
   2 2 3
-> 2 5
-> 7
```
For the last test case, Elsie doesn��t need to perform any operations; the log already consists of equal entries.

