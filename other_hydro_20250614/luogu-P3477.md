## ��Ŀ����
Multiset is a mathematical object similar to a set,    but each member of a multiset may have more than one membership.

Just as with any set, the members of a multiset can be ordered    in many ways. We call each such ordering a permutation    of the multiset. For example, among the permutations of the    multiset{1,1,2,3,3,3,7,8}. there are {2,3,1,3,3,7,1,8}   and{8,7,3,3,3,2,1,1}.

We will say that one permutation of a given multiset is smaller    (in lexicographic order) than another permutation, if on the first    position that does not match the first permutation has a smaller    element than the other one. All permutations of a given multiset    can be numbered (starting from one) in an increasing order.

Task      Write a programme that   reads the description of a permutation of a multiset and a positive          integerm from the standard input,                      determines the remainder of the rank of that permutation in the          lexicographic ordering modulo m,         writes out the result to the standard output.

���ؼ�������ѧ�е�һ��������Ķ�����񼯺ϣ������ڶ��ؼ�֮�У�ͬһ��Ԫ�ؿ��Գ��ֶ�Ρ�


�ͼ���һ�������ؼ��ĵ�Ԫ�ؿ����кܶ���Ԫ�ص��Ų�˳�����ǰ����������ؼ������С�


�������Ƕ�����ؼ���ĳ������$s_i$��ĳ������$s_j$

�Ĵ�С�Ƚ�Ϊ�ֵ���Ƚϡ�����ĳ�����ؼ������п��Դ�С�������������


���ڸ���һ��Ԫ�ظ���Ϊn�Ķ��ؼ���һ�����к�m����������е�����ȡģm��


## �����ʽ
The first line of the standard input holds two integers n($1\le n \le 300000$) and m  ($2 \le m \le 10^9$ ) ,separated by      a single space. These denote, respectively, the cardinality of the      multiset and \dots\ the number m.

The second line of the standard input contains n positive integers      $a_i$($1\le a_i \le 300000$), separated by single spaces and denoting      successive elements of the multiset permutation.

��һ�� ��������n,m


�ڶ��� n������������ؼ�������


## �����ʽ
The first and only line of the standard output is to hold one integer,      the remainder modulo m of the rank of the input permutation in the      lexicographic ordering.


һ��һ������ ����ȡģm


```input1
4 1000
2 1 10 2

```

```output1
5

```

## ��ʾ
��л@Զ��֮�� ���׵ķ���


