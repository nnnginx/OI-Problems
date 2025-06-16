## ��Ŀ����
Bytea went to a salad bar.

There are $n$ fruits one next to another on the bar counter.

Specifically, these are apples and oranges.

Bytea can pick any contiguous part of the line of fruits for her salad.

The fruits she chooses will be added to the salad either from left to right or from right to left.

As Bytea loves oranges, she requires that throughout the salad making process, the number of oranges    in it should always be no smaller than the number of apples, regardless of whether these are added %    from left to right or from right to left.

Help Bytea out by writing a program that will find the longest contiguous part of the line of fruits    that satisfies her requirements.

��һ������Ϊn���ַ�����ÿһλֻ����p��j����һ����Ӵ���ʹ�ò����Ǵ������һ��Ǵ�������ȡ������֤ÿʱÿ����ȡ����p�ĸ�����С��j�ĸ�����


## �����ʽ
The first line of the standard input contains a single integer $n$ ($1\le n\le 1\ 000\ 000$), denoting the number of fruits.

The next line contains a string of $n$ characters $a_1,a_2,\cdots,a_n$ ($a_i\in \{j,p\}$).

These stand for Polish names of apples and oranges: jab\l{ka} and pomara\'ncze).

Consequently, if $a_i=j$, then the $i$-th fruit in a line is an apple,      and otherwise it is an orange.


## �����ʽ
The first and only line of the standard output should contain a single integer equal to the number of fruits in the longest contiguous part of the line that satisfies Bytea's requirements.

Note that it could be the case that $0$ is the correct result.


```input1
6
jpjppj

```

```output1
4

```

## ��ʾ
��һ������Ϊn���ַ�����ÿһλֻ����p��j����һ����Ӵ���ʹ�ò����Ǵ������һ��Ǵ�������ȡ������֤ÿʱÿ����ȡ����p�ĸ�����С��j�ĸ�����


