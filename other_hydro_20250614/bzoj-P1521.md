## ���ⷭ��

����, ������һ���� $n$ ��������ɵ�Ӣ���ı����������Ƕ�����һ������ʼ���һ����ǿո�ָ��������ª��ѹ�д��롣����԰�����ͨ�� $k-1$ �λ��зָ�� $k$ �е��ı���ȥ��������ĩ�ո�Ϊ�������������������һ������Ϊ $k-1$ ������ $\{a_1,a_2,...,a_{k-1}\}$����ʾ�� $1$ ���� $a_1$ �����ʷ��ڵ� $1$ �У��� $a_1+1$����$a_2$ �����ʷ��ڵ� $2$ �У��Դ����ơ�

������Ϊ�����µ��ı����������ϣ��**������ÿһ�еĳ��Ȳ����� $m$ ������������г���֮��ĺ���С**������أ��� $\operatorname{length}(i) $��ʾ��$i$�����ʵĳ��ȣ�$\operatorname{line}(i)$ ��ʾ�� $i$ �еĳ��ȣ���:

$$

\operatorname{line}(i)=(a_i-a_{i-1}-1)+\sum_{j=a_{i-1}+1}^{a_i}\operatorname{length}(j)

$$

����Ҫ��õĴ� $Ans$ Ϊ:

$$

Ans=\min_{k,\operatorname{line}(i)\le m}\{\sum_{i=1}^{k-1}|\operatorname{line}(i)-\operatorname{line}(i+1)|\}

$$

�������뵥���� $n$���г������� $m$ ��ÿ�����ʵĳ��� $\operatorname{length}(i)$��������𰸡�

## �����ʽ

The first line of the standard input contains the numbers $m$ and $n$, $1\le m\le 10^6$,$1\le n\le 2\ 000$, separated by a single space. The second, last line of the standard input contains $n$ integers, denotingthe lengths of subsequent words, $1\le length(i)\le m$ for $i=1,2,\cdots,n$, separated by single spaces.



## �����ʽ

The first and only line of the standard output should contain exactly one integer: the minimumcoefficient of aestheticism for those decompositions, whose every line's length does not exceed $m$.


```input1
6 4
4 3 2 5
```
```output1
3
```