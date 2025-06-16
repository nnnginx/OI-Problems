## ��Ŀ����
Kotori is very good at math (really?) and she loves playing with permutations and primes.

One day, she thinks of a special kind of permutation named $\textit{k co-prime permutation}$. A permutation $p_1,p_2,\cdots,p_n$ of $n$ is called a $k$ co-prime permutation of $n$ if there exists exactly $k$ integers $i$ such that $1 \le i \le n$ and $\text{gcd}(p_i,i)=1$, where $\text{gcd}(x,y)$ indicates the greatest common divisor of $x$ and $y$.

Given $n$ and $k$, please help Kotori construct a $k$ co-prime permutation of $n$ or just report that there is no such permutation.

Recall that a permutation of $n$ is a sequence of length $n$ containing all integers from $1$ to $n$.

## �����ʽ
There is only one test case in each test file.

The first and only line contains two integers $n$ and $k$ ($1 \le n \le 10^6$, $0 \le k \le n$).

## �����ʽ
Output one line containing $n$ integers $p_1, p_2, \cdots, p_n$ separated by one space, indicating the permutation satisfying the given constraints. If no such permutation exists output ``-1`` (without quotes) instead. If there are multiple valid answers you can print any of them.

Please, DO NOT output extra spaces at the end of each line, otherwise your answer may be considered incorrect!

## ��Ŀ����
### ��Ŀ����

������������ $n$ �� $k$������һ�� $1 \sim n$ ������ $p_1,p_2,\cdots,p_n$��ʹ�ô��� $k$ ������ $i$ ���� $1 \le i \le n$ �� $\text{gcd}(p_i,i)=1$��

$\text{gcd}(x,y)$ ��ʾ $x$ �� $y$ �����Լ����

### �����ʽ

ֻ��һ��������ݡ�

��һ�������������� $n$ �� $k$ $(1 \le n \le 10^6, 0 \le k \le n)$��

### �����ʽ

���һ�� $n$ ������ $p_1, p_2, \cdots, p_n$���ÿո�ָ�����ʾһ�����������Լ�������С����û�д��ڵ���������� ``-1``������ж����Ч�Ĵ𰸣��������һ�����ɡ�

�벻Ҫ����ĩ�������Ŀո񣬷�����Ĵ𰸿��ܻᱻ��Ϊ�Ǵ���ġ�

### ���� #1

#### �������� #1

```
5 3
```

#### ������� #1

```
1 4 5 2 3
```

### ���� #2

#### �������� #2

```
1 0
```

#### ������� #2

```
-1
```

```input1
5 3
```

```output1
1 4 5 2 3
```

```input2
1 0
```

```output2
-1
```

