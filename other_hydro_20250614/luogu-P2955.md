## ��Ŀ����
Bessie's cruel second grade teacher has assigned a list of N (1 <= N <= 100) positive integers I (1 <= I <= 10^60) for which Bessie must determine their parity (explained in second grade as 'Even... or odd?'). Bessie is overwhelmed by the size of the list and by the size of the numbers. After all, she only learned to count recently.

Write a program to read in the N integers and print 'even' on a single line for even numbers and likewise 'odd' for odd numbers.

POINTS: 25

Bessie�ǲ����˵��Ķ��꼶��ʦ����һ���� N �������� I �ı��Bessieȥ�жϡ���ż�ԡ������������˼����꼶��ѧ�����ͣ����ǡ�������ǵ���������˫������������Bessie���Ǹ���ĳ���������𾪵��ˣ���Ȼ�������ķ������һ������⣡�����Ͼ����Ÿո�ѧ����������

дһ���������N�������������˫������ô�ڵ�����һ�������"even"������ǵ��������Ƶ����"odd".

���ݷ�Χ��ÿ�������������� ${10}^{60}$��

## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N+1: Line j+1 contains I\_j, the j-th integer to determine even/odd


## �����ʽ
\* Lines 1..N: Line j contains the word 'even' or 'odd', depending on the parity of I\_j


```input1
2 
1024 
5931 

```

```output1
even 
odd 

```

## ��ʾ
Two integers: 1024 and 5931


1024 is eminently divisible by 2; 5931 is not 



