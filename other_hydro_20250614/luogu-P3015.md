## ��Ŀ����
Recently, the cows have been competing with strings of balanced parentheses and comparing them with each other to see who has the best one.

Such strings are scored as follows (all strings are balanced): the string '()' has score 1; if 'A' has score s(A) then '(A)' has score 2\*s(A); and if 'A' and 'B' have scores s(A) and s(B), respectively, then 'AB' has score s(A)+s(B). For example, s('(())()') = s('(())')+s('()') = 2\*s('()')+1 = 2\*1+1 = 3.

Bessie wants to beat all of her fellow cows, so she needs to calculate the score of some strings. Given a string of balanced parentheses of length N (2 <= N <= 100,000), help Bessie compute its score.

����һ��ֻ�����������ŵ��ַ������÷ֹ������£�

���һ��������û�����ţ���ô������ŵĵ÷�Ϊ1������������Ż��������������д��ڣ��������������ŵĵ÷���ӣ���������ڰ���һ�����ţ���ô������ŵĵ÷ּ�Ϊ�ڲ��������еĵ÷�\*2��

���磺��������һ���ַ�����"() ()"���������Ų��д��ڣ���÷�Ϊ1+1=2;

����������һ���ַ�����"(())"�������������ڲ����һ�����ţ���÷�Ϊ2\*1=2.


Bessie���������ͬ�µ�ţ����������Ҫ����ĳ���ַ��������֡�����һ������Ϊn��ֻ�������ŵ��ַ�����2��N��100000����������÷ְ���Bessie��


## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N + 1: Line i+1 will contain 1 integer: 0 if the ith character of the string is '(',  and 1 if the ith character of the string is ')'


## �����ʽ
\* Line 1: The score of the string. Since this number can get quite large, output the  score modulo 12345678910.


```input1
6 
0 
0 
1 
1 
0 
1 

```

```output1
3 

```

## ��ʾ
This corresponds to the string "(())()". 

As discussed above.

�����Ҫmod12345678910


