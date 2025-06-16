## Description

You are given a hint to guess a positive number $x$, an integer ranging from $1$ to $n$.  


## Input

The first line contains a number $n$, indicating the range of the number (from $1$ to $n$).  
The second line contains a Python expression that implies $x$.

## Output

One integer $x$ to get full points. To get a few points without guessing, give a `0` as the answer.

For each case, write your answer into a file `date#.usr`. Either submit them directly within the editor on page, or pack all answer files into a single zip and upload it.

```input1
10
abs(x - 7) == 4
```

```output1
3
```

## Limits And Hints

�����и����� Python ���ʽ�� C++ ������ͬ�����ʽ�� `x` ��һ�����ͱ������� `x` Ϊ��ȷ��ʱ�����ʽ��ֵΪ `True`������Ϊ `False`����֤��Ωһ��

ע��
* Python �� `a ** b` ��ʾ���� $a^b$��
* `pi` ��ֵΪ $3.141592653589793$�����Ǻ���ʹ�û����ơ�
* �����ı��ʽ����ֱ���� Python �� `from math import *` ����ֵ��
* ����Ĳ��������У�`in` �ļ������ $0$ �ɵõķ����ٷֱȣ�`out` �ļ�����ȷ���ڡ����ϴ��ύ������Ŀʱ����� Special Judge ����Ҫ `in`/`out` �ļ������� `data.yml` �ж�Ӧʡ�� `inputFile`/`outputFile` �
* **����֤** ����һ���������ڡ�

