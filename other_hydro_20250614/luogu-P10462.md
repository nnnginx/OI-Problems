## ��Ŀ����
Write a program to convert numbers in one base to numbers in a second base. There are $62$ different digits:

$\{ 0\sim 9, A\sim Z,a\sim z \}$

HINT: If you make a sequence of base conversions using the output of one conversion as the input to the next, when you get back to the original base, you should get the original number.


## �����ʽ
The first line of input contains a single positive integer. This is the number of lines that follow. Each of the following lines will have a (decimal) input base followed by a (decimal) output base followed by a number expressed in the input base. Both the input base and the output base will be in the range from $2$ to $62$. That is (in decimal) $A = 10, B = 11, \dots, Z = 35, a = 36, b = 37, \dots, z = 61$ ($0\sim 9$ have their usual meanings).

## �����ʽ
The output of the program should consist of three lines of output for each base conversion performed. The first line should be the input base in decimal followed by a space then the input number (as given expressed in the input base). The second output line should be the output base followed by a space then the input number (as expressed in the output base). The third output line is blank.

## ��Ŀ����
**����Ŀ������**

��дһ�����򣬽�һ�������е�����ת��Ϊ��һ�������е����֡��� $62$ ����ͬ�����֣�

${ 0\sim 9, A\sim Z,a\sim z }$

��ʾ���������������һϵ�еĽ���ת������һ��ת���������Ϊ��һ��ת�������룬����ص�ԭʼ�Ľ���ʱ����Ӧ�õõ�ԭʼ�����֡�

**�������ʽ��**

����ĵ�һ�а���һ������������ʾ�������ж��������롣��������ÿһ�ж�����һ��������ƣ�ʮ���Ʊ�ʾ����һ��������ƣ�ʮ���Ʊ�ʾ����Ȼ������������Ʊ�ʾ�����֡�������ƺ�������ƶ����� $2$ �� $62$ �ķ�Χ�ڡ�Ҳ����˵��ʮ���Ʊ�ʾ��$A = 10, B = 11, \dots, Z = 35, a = 36, b = 37, \dots, z = 61$����$0\sim 9$ ����˼��ƽ��һ������

**�������ʽ��**

��������Ӧ�ð���ÿ�ν���ת���������������һ��Ӧ������ʮ���Ʊ�ʾ��������ƣ�Ȼ����һ���ո񣬽�������������Ʊ�ʾ���������֡��ڶ��������������ƣ�Ȼ����һ���ո񣬽�������������Ʊ�ʾ���������֡�����������ǿհ��С�

���������ڣ�ChatGPT��

```input1
8
62 2 abcdefghiz
10 16 1234567890123456789012345678901234567890
16 35 3A0C92075C0DBF3B8ACBC5F96CE3F0AD2
35 23 333YMHOUE8JPLT7OX6K9FYCQ8A
23 49 946B9AA02MI37E3D3MMJ4G7BL2F05
49 61 1VbDkSIMJL3JjRgAdlUfcaWj
61 5 dl9MDSWqwHjDnToKcsWE1S
5 10 42104444441001414401221302402201233340311104212022133030
```

```output1
62 abcdefghiz
2 11011100000100010111110010010110011111001001100011010010001

10 1234567890123456789012345678901234567890
16 3A0C92075C0DBF3B8ACBC5F96CE3F0AD2

16 3A0C92075C0DBF3B8ACBC5F96CE3F0AD2
35 333YMHOUE8JPLT7OX6K9FYCQ8A

35 333YMHOUE8JPLT7OX6K9FYCQ8A
23 946B9AA02MI37E3D3MMJ4G7BL2F05

23 946B9AA02MI37E3D3MMJ4G7BL2F05
49 1VbDkSIMJL3JjRgAdlUfcaWj

49 1VbDkSIMJL3JjRgAdlUfcaWj
61 dl9MDSWqwHjDnToKcsWE1S

61 dl9MDSWqwHjDnToKcsWE1S
5 42104444441001414401221302402201233340311104212022133030

5 42104444441001414401221302402201233340311104212022133030
10 1234567890123456789012345678901234567890
```

## ��ʾ
��Ŀ��֤ $1\le T\le 100$��Ҫת���������ǲ����� $10^{110}$ ����Ȼ����

