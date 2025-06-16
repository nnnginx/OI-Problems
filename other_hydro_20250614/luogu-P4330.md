## ��Ŀ����
While debugging a program Mirko noticed that a bug in the program may be linked with the existence of so called square killers in the program memory. The program memory is a matrix composed of R rows and C columns consisting only of zeroes and ones. A square killer is a square submatrix in memory, consisting of more than one character, that, when rotated 180 degrees looks exactly the same. For example, the following matrix contains 3 square killers:

![](https://cdn.luogu.com.cn/upload/pic/15764.png)

Mirko is wondering if there is a connection between the size of the largest square killer and the bug in the program. Help Mirko by writing a program that, given the layout of the memory, outputs the size of the largest square killer. The size of the square killer is the number of rows (or columns) that the killer consists of. In the example above the killer sizes are 2, 2 and 3, respectively.

## �����ʽ
The first will contain two integers, R and C, smaller than or equal to 300.
The next R lines will each contain C characters ('0' or '1') with no spaces.

## �����ʽ
Output the size of the largest killer on a single line, or output -1 if there are no square killers.

## ��Ŀ����
Mirko��дbug��ʱ��ע�⵽����һ�����⣺�����е�bug�������ڴ��еġ�square killer���йء�������ڴ���һ��r��c�е�01���󡣡�square killer�������а���һ��**����**�ַ���һ���������Ӿ��󣬶��ҡ�square killer����ת180�����ԭ����ͬ�����磬����ľ����к���������square killer��:

Mirko��֪�����������ġ�square killer����bug����ϵ��������дһ������������ġ�square killer���Ĵ�С����square killer���Ĵ�С��ָ�����е�������������ͼ�еġ�square killer���Ĵ�С�ֱ���2��2��3��

Translated by @ACdreamer 

```input1
3 6
101010
111001
101001
```

```output1
3
```

```input2
4 5
10010
01010
10101
01001
```

```output2
3
```

```input3
3 3
101
111
100
```

```output3
-1
```

