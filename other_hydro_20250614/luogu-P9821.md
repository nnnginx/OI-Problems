## ��Ŀ����
Given two non-negative integers $X$ and $Y$, determine the value of 
$$ \sum_{i=0}^{X}\sum_{j=[i=0]}^{Y}[i\&j=0]\lfloor\log_2(i+j)+1\rfloor $$
modulo $10^9+7$ where
- $\&$ denotes bitwise AND;
- $[A]$ equals 1 if $A$ is true, otherwise $0$;
- $\lfloor x\rfloor$ equals the maximum integer whose value is no more than $x$.

## �����ʽ
The first line contains one integer $T\,(1\le T \le 10^5)$ denoting the number of test cases.

Each of the following $T$ lines contains two integers $X, Y\,(0\le X,Y \le 10^9)$ indicating a test case.

## �����ʽ
For each test case, print one line containing one integer, the answer to the test case.

## ��Ŀ����
���������Ǹ����� $X,Y$����������ʽ�Ӷ� $10^9+7$ ȡģ��ֵ��
$$
\sum\limits_{i=0}^{X}{\sum\limits_{j=[i=0]}^{Y}{[i \& j=0]\lfloor \log_2(i+j)+1\rfloor}}
$$
���У�

- $\&$ ��ʾ��λ�롣
- $[A]$ ���� $1$�����ҽ������ʽ $A$ Ϊ�棻���� $[A]$ ���� $0$��
- $\lfloor x \rfloor$ ��ʾ������ $x$ �����������

```input1
3
3 3
19 26
8 17
```

```output1
14
814
278
```

## ��ʾ
For the first test case:
- Two $(i,j)$ pairs increase the sum by 1: $(0, 1), (1, 0)$
- Six $(i,j)$ pairs increase the sum by 2: $(0, 2), (0, 3), (1, 2), (2, 0), (2, 1), (3, 0)$

So the answer is $1\times 2 + 2\times 6 = 14$.

