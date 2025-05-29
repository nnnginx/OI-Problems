## ��Ŀ����
Nested quotations are great not only for writing literature with a complex narrative structure, but also in programming languages. While it may seem necessary to use different quotation marks at different nesting levels for clarity, there is an alternative. We can display various nesting levels using $k$-quotations, which are defined as follows.

A $1$-quotation is a string that begins with a quote character, ends with another quote character and contains no quote characters in-between. These are just the usual (unnested) quotations. For example, 'this is a string' is a $1$-quotation.

For $k > 1$, a $k$-quotation is a string that begins with $k$ quote characters, ends with another $k$ quote characters and contains a nested string in-between. The nested string is a non-empty sequence of $(k-1)$-quotations, which may be preceded, separated, and/or succeeded by any number of non-quote characters. For example, ''All 'work' and no 'play''' is a $2$-quotation.

Given a description of a string, you must determine its maximum possible nesting level.

## �����ʽ
The input consists of two lines. The first line contains an integer $n$ ($1 \le n \le 100$). The second line contains $n$ integers $a_1, a_2, \ldots , a_ n$ ($1 \le a_ i \le 100$), which describe a string as follows. The string starts with $a_1$ quote characters, which are followed by a positive number of non-quote characters, which are followed by $a_2$ quote characters, which are followed by a positive number of non-quote characters, and so on, until the string ends with $a_ n$ quote characters.

## �����ʽ
Display the largest number $k$ such that a string described by the input is a $k$-quotation. If there is no such $k$, display no quotation instead.

## ��Ŀ����
���� $1$ ��������һ���������ַ� ' ��ͷ�ͽ�β���м䲻���������ַ����ַ��������� $k$ ������Ϊ���˸������� $k(k>1)$ �����ţ��м������ɸ� $k-1$ �����õ��ַ��������е�һ�� $k-1$ ������ǰ�����һ�� $k-1$ �����ú��������� $k-1$ ������֮�䶼�������������������ַ���

�ָ���һ���ַ����м����������Ŷεĸ��� $n(n\le100)$������ $n$ �������������Ŷεĳ��� $a_1,...,a_n$�������� $k$��ʹ������ַ�����һ�� $k$ �����á�
�������� $k$ �����ڣ���� `no quotation`��

translated by @Starlight237

```input1
5
2 1 1 1 3

```

```output1
2

```

```input2
1
22

```

```output2
4

```

```input3
1
1

```

```output3
no quotation

```

## ��ʾ
Time limit: 2000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2016

