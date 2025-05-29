## ��Ŀ����
The fundamental theorem of arithmetic states that every integer greater than $1$ can be uniquely represented as a product of one or more primes. While unique, several arrangements of the prime factors may be possible. For example:

- $10=2\times 5=5\times 2$��
- $20=2\times 2\times 5=2\times 5\times 2=5\times 2\times 2$��

Let $f(k)$ be the number of different arrangements of the prime factors of $k$. So $f(10) = 2$ and $f(20) = 3$.

Given a positive number $n$, there always exists at least one number $k$ such that $f(k) = n$. We want to know the smallest such $k$.

## �����ʽ
The input consists of at most $1 000$ test cases, each on a separate line. Each test case is a positive integer $n < 2^{63}$.

## �����ʽ
For each test case, display its number $n$ and the smallest number $k > 1$ such that $f(k) = n$. The numbers in the input are chosen such that $k < 2^{63}$.

## ��Ŀ����
**����Ŀ������**

������������ָ����ÿ������ $1$ ������������Ψһ��ʾΪһ�����������ĳ˻�����Ȼ��ʾ��Ψһ�ģ����������ӵ����п����ж��֡����磺

- $10=2\times 5=5\times 2$��
- $20=2\times 2\times 5=2\times 5\times 2=5\times 2\times 2$��

�� $f(k)$ Ϊ $k$ ���������Ӳ�ͬ���е���������ˣ�$f(10) = 2$ �� $f(20) = 3$��

����һ�������� $n$���������ٴ���һ������ $k$ ʹ�� $f(k) = n$��������֪����С�������� $k$��

**�������ʽ��**

���������� $1 000$ ������������ÿ����������ռһ�С�ÿ������������һ�������� $n < 2^{63}$��

**�������ʽ��**

����ÿ��������������������� $n$ �Լ���С�� $k > 1$ ʹ�� $f(k) = n$�������е�����ѡ��ʹ�� $k < 2^{63}$��

���������ڣ�[ChatGPT](https://chatgpt.com/)��


```input1
1
2
3
105
```

```output1
1 2
2 6
3 12
105 720
```

