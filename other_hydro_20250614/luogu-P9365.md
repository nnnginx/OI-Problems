## ��Ŀ����
$$
2 ^ {2 ^ {2 ^ {2 ^ {2 ^ {2 ^ {2 ^ {2 ^ {2 ^ {2}}}}}}}}}
$$

SolarPea likes blowing up PolarSea's blog by sending power tower of $2$. As the tower is too high, the stack of the web page overflows. So the blog no longer works.

Now SolarPea has $n$ powers of two $a_1, a_2, \ldots, a_n$, $x$ bitwise AND operators, $y$ bitwise OR operators and $z$ bitwise XOR operators. It is guaranteed that $n = x + y + z$.

Solarpea wants to construct an arithmetic expression with these numbers and operators. Formally, define $x_0 = 0$ and $x_i = x_{i - 1}\ \mathrm{op}_i\ b_i$, where $b$ is a permutation of $a$, which means we can rearrange $a$ to get $b$, and $\mathrm{op}_i$ is one of the three types of bitwise operators above. Then $x_n$ is the result of the expresstion.

The larger the expression, the more likely it is to make PolarSea's blog unable to work. SolarPea wants you to help him to find the largest $x_n$ and construct such an expression. If there are multiple solutions, output any of them.

You need to process $T$ test cases independently.

## �����ʽ
The first line contains a single integer $T$ ($1\leq T \leq 10 ^ 5$), denoting the number of test cases.

For each test case, the first line contains four integers $n$, $x$, $y$ and $z$ ($0\leq x, y, z\leq n \leq 65\,536, n = x + y + z$). The next line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($0\leq c_i < n$), where $a_i = 2 ^ {c_i}$.

It is guaranteed that the sum of $n$ over all test cases is no more than $1\,048\,576$.

## �����ʽ
For each test case, output three lines.

The first line contains a $01$-string of length $n$, representing the binary form of the largest $x_n$.

The next line contains a single $1$-indexed string $\mathrm{op}$ of length $n$, where $\mathrm{op}_i$ represents the $i$-th operator. Here, we denote AND as `&` (ASCII 38), OR as `|` (ASCII 124), and XOR as `^` (ASCII 94). You should guarantee that there is exactly $x$ AND operators, $y$ OR operators and $z$ XOR operators.

The third line contains $n$ integers $d_1, d_2, \ldots, d_n$, the $i$-th of which representing the logarithm of $b_i$ with base $2$. That is, $d$ is a permutaion of $c$.

If there are multiple solutions, output any of them.

## ��Ŀ����
## ��Ŀ����
SolarPea ϲ��ͨ�����͵�������ը�� PolarSea �Ĳ��� $2$��������̫�ߣ���ҳ�Ķ�ջ��������Բ����Ѿ��������ˡ�  

���� SolarPea ӵ������ $a_1��a_2��ldots��a_n$��$x$ λ AND �������$y$ λ OR ������� $z$ λ XOR ������� $n$ �η�����֤ $n = x + y + z$��  

Solarpea ϣ��ʹ����Щ���ֺ����������һ���������ʽ����ʽ�ض��� $x_0 = 0$ �� $x_i = x_{i - 1}\ \mathrm{op}_i\ b_i$������ $b$ �� $a$ �����У�����ζ�����ǿ����������� $a$ ���õ� $b$���� $\mathrm{op}_i$ �������������͵İ�λ�����֮һ����ô $x_n$ ���Ǳ��ʽ�Ľ����

���ʽԽ�󣬾�Խ�п���ʹ PolarSea �Ĳ����޷�������SolarPea ϣ��������ҵ����� $x_n$ �����������ı��ʽ������ж���������������������κ�һ����

����Ҫ�������� $T$ ������������
## �����ʽ
��һ�а���һ������ $T $ ��$1\leq T \leq 10 ^ 5$������ʾ����������������  

����ÿ��������������һ�а����ĸ����� $n$�� $x$�� $y$ �� $z$ ��$0\leq x, y, z\leq n \leq 65\,536, n = x + y + z$������һ�а��� $n$ ������ $c_1, c_2, \ldots, c_n$ ($0\leq c_i < n$)������ $a_i = 2 ^ {c_i}$��

��֤���в��������� $n $ ֮�Ͳ����� $1\,048\,576$��  
## �����ʽ
����ÿ��������������� 3 �С�  

��һ�а���һ������Ϊ $n$ �� $01$ �ַ�������ʾ��� $x_n$ �Ķ�������ʽ��  

��һ�а���һ������Ϊ $n$ �� $1$ �����ַ��� $\mathrm{op}$������ $\mathrm{op}_i$��ʾ�� $i$ �����������������ǽ� AND ��ʾΪ `&` ��ASCII 38����OR ��ʾΪ `|` ��ASCII 124������ XOR ��ʾΪ `^` ��ASCII 94������Ӧ�ñ�֤������ $x $ AND �������$y$ OR ������� $z$ XOR �������

�����а��� $n$ ������ $d_1, d_2, \ldots, d_n$�����е� $i$ ������ $b_i$ �Ķ������� $2$ Ϊ�ס�Ҳ����˵��$d$ �� $c$ �����С�

����ж���������������������κ�һ����

## �����������
��
## ��ʾ
**��Դ**��2022 ICPC ����ϰ������������ H.  
**����**�� Alex_Wei.

```input1
4
4 3 0 1
1 0 1 0
4 1 0 3
1 0 1 0
8 0 2 6
1 5 5 7 1 5 5 7
8 0 0 8
1 5 5 7 1 5 5 7

```

```output1
0010
&&^&
0 0 1 1
0011
^^&^
0 1 0 1
10100000
^^|^^^^|
1 5 5 7 1 5 5 7
00000000
^^^^^^^^
1 5 5 7 1 5 5 7

```

## ��ʾ
**Source**: The 2022 ICPC Asia Xi'an Regional Contest Problem H.

**Author**: Alex_Wei.

![](https://cdn.luogu.com.cn/upload/image_hosting/g2frgx9s.png)

