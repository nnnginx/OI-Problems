## ��Ŀ����
Prof. Pang has $n$ rectangles, the coordinate of the lower left corner of the $i$-th rectangle is $(x_{i,1}, y_{i,1})$, and the coordinate of the upper right corner is $(x_{i,2}, y_{i,2})$. Rectangles may overlap.

You need to choose three straight lines such that:

- Each line should be parallel to the $x$-axis or the $y$-axis, which means its formula is $x = a$ or $y = a$.
- In the formula $x = a$ or $y = a$, $a$ should be an integer in $[1, 10^9]$.
- These three lines should be distinct.
- Each rectangle is $\textbf{touched}$ by at least one line. A line touches a rectangle if it intersects with the boundary and/or the interior of the rectangle.

You need to compute the number of ways to choose three lines. Since the answer can be very large, output it modulo $998244353$. Two ways are considered the same if only the order of three lines differs in these two ways. 

## �����ʽ
The first line contains a single integer $T~(1 \le T \le 10^5)$, denoting the number of test cases.

For each test case, the first line contains an integer $n~(1 \le n \le 10^5)$. The $i$-th line of the next $n$ lines contains four integers $x_{i,1}, y_{i,1},x_{i,2}, y_{i,2}~(1\le x_{i,1}<x_{i,2}\le 10^9,1\le y_{i,1}<y_{i,2}\le 10^9)$.

It is guaranteed that the sum of $n$ over all test cases does not exceed $2\times 10^5$.

## �����ʽ
For each test case, output one integer representing the answer in one line.

## ��Ŀ����
**����Ŀ������**

�ӽ����� $n$ �����Σ��� $i$ �����ε����½������� $(x_{i,1}, y_{i,1})$�����Ͻ������� $(x_{i,2}, y_{i,2})$�����ο����ص���

����Ҫѡ������ֱ�ߣ�ʹ�ã�

- ÿ��ֱ��Ӧ���� $x$ ��� $y$ ��ƽ�У����䷽��Ϊ $x = a$ �� $y = a$��
- �ڷ��� $x = a$ �� $y = a$ �У�$a$ Ӧ���� $[1, 10^9]$ �����ڵ�������
- ������ֱ��Ӧ���ǲ�ͬ�ġ�
- ÿ���������ٱ�һ��ֱ�� $\textbf{����}$�����һ��ֱ������εı߽��/���ڲ��ཻ����Ƹ�ֱ�ߴ����þ��Ρ�

����Ҫ����ѡ������ֱ�ߵķ����������ڴ𰸿��ܷǳ�������� $998244353$ ȡģ�Ľ����������ַ���ֻ������ֱ�ߵ�˳��ͬ������Ϊ��������ͬ�ġ�

**�������ʽ��**

��һ�а���һ������ $T~(1 \le T \le 10^5)$����ʾ����������������

����ÿ��������������һ�а���һ������ $n~(1 \le n \le 10^5)$���������� $n$ ���У��� $i$ �а����ĸ����� $x_{i,1}, y_{i,1},x_{i,2}, y_{i,2}~(1\le x_{i,1}<x_{i,2}\le 10^9,1\le y_{i,1}<y_{i,2}\le 10^9)$��

��֤���в��������� $n$ ���ܺͲ����� $2\times 10^5$��

**�������ʽ��**

����ÿ���������������һ����������ʾ�𰸡�

**���������͡�**

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
3
1
1 1 1000000000 1000000000
3
1 1 2 2
3 3 4 4
5 5 6 6
5
581574116 47617804 999010750 826131769
223840663 366320907 613364068 926991396
267630832 51913575 488301124 223957497
217461197 492085159 999485867 913732845
28144453 603781668 912516656 993160442
```

```output1
230616300
64
977066618
```

