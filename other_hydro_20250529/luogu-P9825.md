## ��Ŀ����
In mathematics, the Fibonacci numbers, commonly denoted as $f_n$, is a sequence such that each number is the sum of the two preceding numbers, starting with $1$ and $1$. That is, $f_1 = 1, f_2 = 1$ and $f_n = f_{n-2} + f_{n-1}~(n \ge 3)$.

Thus, the beginning of the sequence is $1, 1, 2, 3, 5, 8, 13, 21,\ldots$ .

Given $n$, please calculate $\sum_{i=1}^{n}{\sum_{j=i+1}^{n}{g(f_i,f_j)}}$, where $g(x,y) = 1$ when $x \cdot y$ is even, otherwise $g(x,y) = 0$.

## �����ʽ
The only line contains one integer $n~(1\le n\le 10^9)$.

## �����ʽ
Output one number -- $\sum_{i=1}^{n}{\sum_{j=i+1}^{n}{g(f_i,f_j)}}$.

## ��Ŀ����
����ѧ�У�쳲��������г�����Ϊ���� $f_n$�������е����� $f_1,f_2$ ��Ϊ $1$����������ƹ�ʽ $f_n=f_{n-2}+f_{n-1}(n\ge 3)$��

��ˣ����е�ǰһЩ��Ϊ $1,1,2,3,5,8,13,21,\cdots$��

�� $x\cdot y$ Ϊż�������� $g(x,y)=1$������ $g(x,y)=0$���� $\sum\limits_{i=1}^n{\sum\limits_{j=i+1}^n{g(f_i,f_j)}}$ ��ֵ��

```input1
3
```

```output1
2
```

```input2
10
```

```output2
24
```

```input3
100
```

```output3
2739
```

