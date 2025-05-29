## ��Ŀ����


Eva is a third-grade elementary school student. She has just learned how to perform addition and subtraction of arbitrary-precision integers. Her homework is to evaluate some expressions. It is boring, so she decided to add a little trick to the homework. Eva wants to add some plus and minus signs to the expression to make its value as large as possible.



## �����ʽ


The single line of the input file contains the original arithmetic expression. It contains only digits, plus $(��+')$ and minus $(��-')$ signs.

The original expression is correct, that is:

numbers have no leading zeroes;

there are no two consecutive signs;

the last character of the expression is a digit.

The length of the original expression does not exceed $1000$ characters.



## �����ʽ


Output a single line -- the original expression with some plus and minus signs added. Output expression must satisfy the same correctness constraints as the original one. Its value must be as large as possible.



## ��Ŀ����
## ��Ŀ���� ##

����һ�������мӼ��ź����ֵı��ʽ�����һЩ�ӺŻ���ţ� ʹ�ò������**�Ϸ�**���ʽ��ֵ��� �����������ı��ʽ��

��һ�����ʽ�Ϸ�ʱ��������������

1.ÿһ������**����ǰ����**��

2.���ʽ��û������**�����ķ���**��

3.���ʽ�����һ���ַ������֡�

��֤ԭʼ���ʽ�ǺϷ��ģ� �ҳ��Ȳ����� $1000$��




```input1
10+20-30

```

```output1
10+20-3+0

```

```input2
-3-4-1

```

```output2
-3-4-1

```

```input3
+10

```

```output3
+10

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



