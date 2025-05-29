## ��Ŀ����

There is a random sequence $L$ whose element are all random numbers either $-1$ or $1$ with the same possibility��Now we define MAVS��the abbreviate of Maximum Absolute Value Subsequence��to be any ��if more than one�� subsequences of $L$ whose absolute value is maximum among all subsequences��Given the length of $L$��your task is to find the expectation of the absolute value of MAVS��

## �����ʽ

There is only one input file��The first line is the number of test cases $T$��$T$ positive integers follow��each of which contains one positive number not greater than $1500$ denoted the length of $L$��

����һ������ $L$���������ִ�����������ִ�ÿ��Ԫ��Ϊ $1$ �� $-1$��  
��ô������������� $2^L$ �ֿ��ܡ�  
�ֶ�ÿ�����ܵ����ִ������������Ӵ��ͣ�������ȡ����ֵ�����������Ǹ�ֵ��  
�����������Щֵ���ܺ͡�  
�����ܺ�/ $2^L$��  

## �����ʽ

For each test case��output the expectation you are required to calculate��Answers are rounded to $6$ numbers after the decimal point����as shown in the sample output��

```input1
3
1
5
10
```

```output1
Case 1: 1.000000
Case 2: 2.750000
Case 3: 4.167969
```

## ��ʾ

������2ʱ����  
```
1 1
1 -1
-1 1
-1 -1
```  
�����ֿ��ܣ����Ӧ��ֵ�ֱ�Ϊ $2+1+1+2=6$��  
$6/4=1.5$

## ��Ŀ��Դ

acm 2011 ����


