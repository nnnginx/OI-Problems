


## ��Ŀ����
Farmer John's N cows, conveniently numbered 1��N, are all standing in a row (they seem to do so often that it now takes very little prompting from Farmer John to line them up). Each cow has a breed ID: 1 for Holsteins, 2 for Guernseys, and 3 for Jerseys. Farmer John would like your help counting the number of cows of each breed that lie within certain intervals of the ordering.
����һ������ΪN�����У�ÿ��λ���ϵ���ֻ������1��2��3�е�һ�֡�
��Q��ѯ�ʣ�ÿ�θ���������a,b����ֱ��������[a,b]������1��2��3�ĸ�����
## �����ʽ
The first line of input contains NN and QQ (1��N��100,000 1��Q��100,000).
The next NN lines contain an integer that is either 1, 2, or 3, giving the breed ID of a single cow in the ordering.
The next QQ lines describe a query in the form of two integers a,b (a��b).
## �����ʽ
For  each of the QQ queries (a,b), print a line containing three numbers:  the number of cows numbered a��b that are Holsteins (breed 1), Guernseys  (breed 2), and Jerseys (breed 3).

```input1
6 3
2
1
1
3
2
1
1 6
3 3
2 4

```
```output1
3 2 1
1 0 0
2 0 1
```

## ��ʾ
û��д����ʾ
## ��Ŀ��Դ
Silver��лClaris�ṩ����


