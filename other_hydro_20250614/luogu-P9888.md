## ��Ŀ����
BaoBao is now learning a new binary operation between two positive integers, represented by $\otimes$, in his magic book. The book tells him that the result of such operation is calculated by concatenating all multiple results of each digit in the two integers.

Formally speaking, let the first integer be $A = a_1a_2 \dots a_n$, where $a_i$ indicates the $i$-th digit in $A$, and the second integer be $B = b_1b_2 \dots b_m$, where $b_i$ indicates the $i$-th digit in $B$. We have 

$$A \otimes B = \sum\limits_{i=1}^n\sum\limits_{j=1}^m a_ib_j = a_1b_1 + a_1b_2 + \dots + a_1b_m + a_2b_1 + \dots + a_nb_m$$ 

Note that the result of $a_ib_j$ is considered to be a $\textbf{string}$ (without leading zeros if $a_ib_j > 0$, or contains exactly one `0` if $a_ib_j = 0$), NOT a normal integer. Also, the sum here means $\textbf{string concatenation}$, NOT the normal addition operation.

For example, $23 \otimes 45 = 8101215$. Because $8=2 \times 4$, $10=2 \times 5$, $12=3 \times 4$ and $15=3 \times 5$.

BaoBao is very smart and soon knows how to do the inverse operation of $\otimes$. Now he gives you the result of a $\otimes$ operation and the numbers of digits in the two original integers. Please help him to restore the two original integers $A$ and $B$.


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains two positive integers $n$ and $m$ ($1 \le n, m \le 2 \times 10^5$), where $n$ indicates the length of $A$ and $m$ indicates the length of $B$. Here length of an integer means the length of the string when writing the number in decimal notation without leading zeros.

The second line contains only one positive integer $C$ without leading zeros, indicating the result of $A \otimes B$. The length of $C$ is no more than $2 \times 10^5$.

It's guaranteed that the sum of lengths of $C$ over all test cases will not exceed $2 \times 10^6$.

## �����ʽ
For each test case output one line.

If there exist such $A$ and $B$ that $A \otimes B = C$, output one line containing two integers $A$ and $B$ separated by one space. Note that $A$ and $B$ should be positive integers without leading zeros, the length of $A$ should be exactly $n$, and the length of $B$ should be exactly $m$.

If there are multiple valid answers, output the answer with the smallest $A$; If there are still more than one answer, output one of them with the smallest $B$.

If such $A$ and $B$ do not exist, print ``Impossible`` (without quotes) on a single line.

## ��Ŀ����
BaoBao ������������ħ������ѧϰ����������֮���һ���µĶ��������㣬�� $\otimes$ ��ʾ���Ȿ�����������������Ľ����ͨ��������������ÿ�����ֵ����ж�����������������ġ�

��ʽ�Ͻ����õ�һ������Ϊ $A=A_1a_2\dots A_n$������ $A_i$ ��ʾ $A$ �еĵ� $i$ λ���ڶ�������Ϊ $B=B_1b_2\dots B_m$������ $B_i$ ��ʾ $B$ �еĵ�һλ��������

$$A \otimes B = \sum\limits_{i=1}^n\sum\limits_{j=1}^m a_ib_j = a_1b_1 + a_1b_2 + \dots + a_1b_m + a_2b_1 + \dots + a_nb_m$$

��ע�⣬$a_ib_j$ �Ľ������Ϊ�� $\textbf{string}$����� $a_ib_j>0$���򲻴�ǰ���㣬������� $a_ib_j > 0$���������һ�� $0$�����������������������⣬����� sum ��ʾ $\textbf{string concatenation}$�������������ļӷ����㡣

���磬$23\otimes 45=8101215$����Ϊ $8=2\times 4$��$10=2\times 5$��$12=3\times 4$ �� $15=3\times 5$��

BaoBao �ܴ������ܿ��֪������� $\otimes$ �������㡣���ڣ��������� $\otimes$ ����Ľ���Լ�����ԭʼ�����е�λ������������ָ�����ԭʼ���� $A$ �� $B$��

## �����ʽ

�ж����������������ĵ�һ�а���һ������ $T$����ʾ��������������������ÿ������������

��һ�а������������� $n$ �� $m$��$1\le n,m\le 2\times 10^5$�������� $n$ ��ʾ $A$ �ĳ��ȣ�$m$ ��ʾ $B$ �ĳ��ȡ���������ĳ�����ָ�ڲ���ǰ�����ʮ���Ƽ�������д������ʱ�ַ����ĳ��ȡ�

�ڶ���ֻ����һ������ǰ����������� $C$����ʾ $A\otimes B$ �Ľ����$C$ �ĳ��Ȳ����� $2\times 10^5$��

��֤���в��������� $C$ �����ܺͲ��ᳬ�� $2\times 10^6$��

## �����ʽ

����ÿ�������������һ�С�

������������� $A$ �� $B$��$A\otimes B=C$�������һ�У����а�����һ���ո�ָ����������� $A$ �� $B$����ע�⣬$A$ �� $B$ Ӧ���ǲ���ǰ�������������$A$ �ĳ���Ӧ�������� $n$��$B$ �ĳ���Ӧ������ $m$��

������ڶ����Ч�𰸣������������С $A$ �Ĵ𰸣������Ȼ��һ�����ϵĴ𰸣����������һ����С�� $B$��

��������������� $A$ �� $B$�����ڵ����ϴ�ӡ ``Impossible``���������ţ���

```input1
4
2 2
8101215
3 4
100000001000
2 2
80101215
3 4
1000000010000
```

```output1
23 45
101 1000
Impossible
Impossible
```

