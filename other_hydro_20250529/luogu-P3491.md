## ��Ŀ����
Let $h$ be a function acting on strings composed of the digits 0 and 1. The function $h$ transforms the string $w$ by replacing (independently and concurrently) every digit 0 with 1 and every digit 1 with the string "10". For example $h("1001") = "101110"$, $h("") = ""$ (i.e. $h$ assigns an empty string to the empty string). Note that $h$ is an injection, or a one - to - one function. By $h^k$ we denote the function $h$ composed with itself $k$ times. In particular, $h^0$ is the identity function $h^0(w)=w$.

We are interested in the strings of the form $h^k("0")$ for $k = 0,1,2,3,\cdots$. This sequence begins with the following strings:

"0", "1", "10", "101", "10110", "10110101".

We call the string $x$ a substring of the string $y$ if it occurs in $y$ as a contiguous (i.e. one - block) subsequence. A sequence of integers $k_1,k_2,\cdots,k_n$ is given. Your task is to check whether a string of the form $h^{k_1}("0") \cdot h^{k_2}("0") \cdots h^{k_n}("0")$ is a substring of $h^m("0")$ for some $m$.

## �����ʽ
The first line of the standard input contains a single integer $t$, $1 \leq t \leq 13$, denoting the number of test units. The first line of each test unit's description contains one integer $n$, $1 \leq n \leq 100000$. The second line of each description holds $n$ non - negative integers $k_1,k_2,\cdots,k_n$, separated by single spaces. The sum of the numbers in the second line of any test unit description does not exceed 10000000.

## �����ʽ
Your programme should print out $t$ lines to the standard output, one for each test unit. Each line corresponding to a test unit should contain one word: TAK (yes in Polish - if $h^{k_1}("0") \cdot h^{k_2}("0") \cdots h^{k_n}("0")$ is a substring of $h^m("0")$ for some $m$ in that test unit, or NIE (no in Polish) otherwise. 

## ��Ŀ����
## ��Ŀ����

����  $h$ ������������  $0$ ��  $1$ ��ɵ��ַ�������ͨ����ÿһ������  $0$ �滻Ϊ  $1$����ÿһ������  $1$ �滻Ϊ�ַ���  $10$ ��������ͬʱ�ر任�ַ���  $w$��

���磺

 $$h(``1001")=``101110"$$
 $$h(``\ ")=``\ "$$

�����������ѿ��ַ�����ֵ�����ַ�����

ע�⣬ $h$ ��һ��һ��һ�ĺ�����

������  $h^k$ ��ʾ����  $h$ ʹ��  $k$ �Ρ�

�ر�ģ� $h^0(w)=w$�� 

���Ƕ�  $k = 0, 1, 2, ...$ ��  $h^k(``0")$ ��ʽ���ַ�������Ȥ���������Ϊ:

 $$ ``0", ``1", ``10", ``101", ``10110", ``10110101", \ldots $$

����ַ���  $x$ ��  $y$ ����һ�������ģ���һ���飩�Ӵ����֣����Ǿͳ�  $x$ Ϊ�ַ���  $y$ ���Ӵ�����������  $k_1, k_2, k_3, ..., k_n $ �����С���������Ǽ���Ƿ���  $m$ ��ʹ $h^{k_1}(``0") \cdot h^{k_2}(``0") \cdot \ldots \cdot h^{k_n}(``0") $ ��ʽ���ַ�����  $h^m(``0")$ ���Ӵ��� 

## ��������
����ĵ�һ�а���һ������  $t$ ��ʾ��������  $1 \leq t \leq 13$��ÿ�������������У�һ��  $n$ �� $1 \leq n \leq 100000$ ����һ��Ϊ  $n$ ���Ǹ�����  $k_1, k_2, k_3, ..., k_n $���õ����ո�ָ���

## �������
���ĳ���Ӧ�����  $t$ �У�ÿ���������һ�С��������  $m$ ʹ  $h^{k_1}(``0") \cdot h^{k_2}(``0") \cdot \ldots \cdot h^{k_n}(``0") $ ��  $h^m(``0")$ ���Ӵ�������� `TAK`���������е� _yes_ �������������  $m$������� `NIE`���������е� _no_ ����

_Translated By in\_young\_ren_ 

```input1
2
2
1 2
2
2 0

```

```output1
TAK
NIE

```

