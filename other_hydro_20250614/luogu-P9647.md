## ��Ŀ����
BaoBao and his $(n-1)$ classmates are going to the park. For convenience, their teacher DreamGrid has numbered the students from 1 to $n$ and decides to form the students into some groups, where each group consists of exactly two students.

For some reason, DreamGrid requires that the indices of the two students in the same group should have a common divisor greater than 1. Note that each student can only belong to at most one group, and it's not necessary that every student belongs to a group.

Please help DreamGrid form as many groups as possible.


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first and only line contains an integer $n$ ($1 \le n \le 10^5$), indicating the number of students.

It's guaranteed that the sum of $n$ of all test cases will not exceed $10^6$.


## �����ʽ
For each test case output one line. The line first contains an integer $k$ indicating the number of groups, then $2k$ integers $a_1, a_2, \dots, a_{2k}$ follow, indicating that student $a_1$ and $a_2$ belong to the same group, student $a_3$ and $a_4$ belong to the same group, ..., student $a_{2k-1}$ and $a_{2k}$ belong to the same group. The integers in a line are separated by a space. If there are multiple valid answers, you can print any of them.

Please, DO NOT output extra spaces at the end of each line, or your solution may be considered incorrect!

## ��Ŀ����
**����Ŀ������**

���������� $(n-1)$ ��ͬѧҪȥ��԰��Ϊ�˷��㣬���ǵ���ʦ������ӽ�ѧ���� 1 �� $n$ ��ţ���������ѧ���ֳ�һЩС�飬ÿ��ǡ��������ѧ����ɡ�

����ĳ��ԭ���������Ҫ��ͬ�������ѧ���ı�ű�����һ������ 1 �Ĺ�Լ����ע�⣬ÿ��ѧ�����ֻ������һ��С�飬���Ҳ���Ҫÿ��ѧ��������һ��С�顣

��������������ɾ����ܶ��С�顣


**�������ʽ��**

�ж����������������ĵ�һ�а���һ������ $T$����ʾ��������������������ÿ������������

��һ����Ψһһ�а���һ������ $n$ ($1 \le n \le 10^5$)����ʾѧ����������

��֤���в��������� $n$ ֮�Ͳ����� $10^6$��

**�������ʽ��**

����ÿ���������������һ�С��������Ȱ���һ������ $k$����ʾС���������Ȼ���� $2k$ ������ $a_1, a_2, \dots, a_{2k}$����ʾѧ�� $a_1$ �� $a_2$ ����ͬһС�飬ѧ�� $a_3$ �� $a_4$ ����ͬһС�飬�Դ����ơ����ڵ������ɿո�ָ�������ж����Ч�𰸣�������������κ�һ����

�벻Ҫ��ÿ�е�ĩβ�������Ŀո񣬷�����Ľ���������ܻᱻ��Ϊ����ȷ��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
3
1
4
6

```

```output1
0
1 2 4
2 2 4 3 6

```

