## ��Ŀ����
Given $n$ intervals $[l_1, r_1], [l_2, r_2], \dots, [l_n, r_n]$, one must select an integer from each of the intervals and calculate their bitwise and value $b$. What's the maximum possible $b$ one can get?


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($1 \le n \le 10^5$), indicating the number of intervals.

For the following $n$ lines, the $i$-th line contains two integers $l_i$ and $r_i$ ($0 \le l_i \le r_i \le 10^9$), indicating the $i$-th interval.

It's guaranteed that the sum of $n$ of all test cases will not exceed $10^6$.


## �����ʽ
For each test case output one line containing one integer, indicating the maximum possible $b$ one can get.


## ��Ŀ����
**����Ŀ������**

���� $n$ ������ $[l_1, r_1], [l_2, r_2], \dots, [l_n, r_n]$����Ҫ��ÿ��������ѡ��һ���������������ǵİ�λ��ֵ $b$���ܹ��õ������ $b$ �Ƕ��٣�

**�������ʽ��**

�ж����������������ĵ�һ�а���һ������ $T$����ʾ��������������������ÿ������������

��һ�а���һ������ $n$ ($1 \le n \le 10^5$)����ʾ�����������

�������� $n$ �У��� $i$ �а����������� $l_i$ �� $r_i$ ($0 \le l_i \le r_i \le 10^9$)����ʾ�� $i$ �����䡣

��֤���в��������� $n$ ֮�Ͳ����� $10^6$��

**�������ʽ��**

����ÿ�������������һ�У�����һ����������ʾ�ܵõ��������� $b$��

**���������͡�**

���ڵ�һ�������������������Դ�����������ѡ�� 7��6 �� 7�����õ����ǵİ�λ��ֵ 6��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
2
3
0 8
2 6
3 9
1
1 100

```

```output1
6
100

```

## ��ʾ
For the first sample test case, one can select 7, 6 and  7 from the three intervals and get their bitwise and value 6.

