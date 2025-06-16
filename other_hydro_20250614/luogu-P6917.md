## ��Ŀ����
Every day, Danny buys one sweet from the candy store and eats it. The store has $m$ types of sweets, numbered from $1$ to $m$. Danny knows that a balanced diet is important and is applying this concept to his sweet purchasing. To each sweet type $i$, he has assigned a target fraction, which is a real number $f_ i$ ($0 < f_ i \le 1$). He wants the fraction of sweets of type $i$ among all sweets he has eaten to be roughly equal to $f_ i$. To be more precise, let $s_ i$ denote the number of sweets of type $i$ that Danny has eaten, and let $n = \sum _{i=1}^ m s_ i$. We say the set of sweets is balanced if for every $i$ we have

\[ n f_ i - 1 < s_ i < n f_ i + 1. \] 

Danny has been buying and eating sweets for a while and during this entire time the set of sweets has been balanced. He is now wondering how many more sweets he can buy while still fulfilling this condition. Given the target fractions $f_ i$ and the sequence of sweets he has eaten so far, determine how many more sweets he can buy and eat so that at any time the set of sweets is balanced.

## �����ʽ
The input consists of three lines. The first line contains two integers $m$ ($1 \le m \le 10^5$), which is the number of types of sweets, and $k$ ($0 \le k \le 10^5$), which is the number of sweets Danny has already eaten.

The second line contains $m$ positive integers $a_1, \ldots , a_ m$. These numbers are proportional to $f_1, \ldots , f_ m$, that is, $\displaystyle f_ i = \frac{a_ i}{\sum _{j = 1}^ m a_ j}$. It is guaranteed that the sum of all $a_ j$ is no larger than $10^5$.

The third line contains $k$ integers $b_1, \ldots , b_ k$ ($1 \le b_ i \le m$), where each $b_ i$ denotes the type of sweet Danny bought and ate on the $i^\text {th}$ day. It is guaranteed that every prefix of this sequence (including the whole sequence) is balanced.

## �����ʽ
Display the maximum number of additional sweets that Danny can buy and eat while keeping his diet continuously balanced. If there is no upper limit on the number of sweets, display the word forever.

## ��Ŀ����
## ��Ŀ����

ÿ�죬Danny ������ǹ�����һ���ǲ��Ե������ǹ������� $m$ ���ǣ����Ϊ $1 \dots m$ ��

Danny ֪��������ʳ����Ҫ�������ڳ����ڹ����ǹ�ʱ��һ���������ʳ���������ÿ���� $i$ ������һ��Ŀ����� $f_i (0 \le f_i \le 1, f_i$ Ϊһ��ʵ�� $) $, ����ϣ�������Ե��������У��� $i$ ���ǵ�����ռ�ȴ��Ϊ $f_i$ ��

׼ȷ��˵�� �� $s_ i$ ��ʾ Danny �Ѿ��Ե��ĵ� $i$ ���ǵ�����,  $n = \sum _{i=1}^ m s_ i$, ������Ϊһ�ֳ��ǵķ����Ǿ���Ľ����������е� $i$�����㣺

$$n f_ i - 1 < s_ i < n f_ i + 1$$

Danny �Ѿ����򲢳Ե���һЩ�ǣ���������֤ÿ��ǰ׺����ʳ���Ǿ���ġ�����֪���ڱ�֤ÿ��ǰ׺������ʳ�������£�����໹�ܳԶ��ٿ��ǡ�

����Ŀ����� $f_i$
�����Ѿ��Թ����ǹ����У�����ȷ���ڱ�֤ÿ��ǰ׺������ʳ�������£�Danny ��໹�ܹ��򲢳Ե����ٿ��ǹ���

## �����ʽ

����������С���һ�а����������� m $1 \le m \le 10^5$ ��ʾ�ǹ�������, $k(0 \le k \le 10^5)$ ��ʾ Danny �Ѿ��Ե����ǹ�������

�ڶ��а��� $m$ �������� $a_1 \dots a_m$, ��   $ \displaystyle f_ i = \frac{a_ i}{\sum _{j = 1}^ m a_ j}$, ��֤
$\sum_{i=1}^m a_i \le 10^5$ ��

�����а��� $k$ �������� $b_1 \dots b_k (1 \le b_i \le m)$, ��ʾ Danny �ڵ� $i$ �칺�򲢳Ե����ǵ����ࡣ��֤���е�ÿ��ǰ׺�������������У�����ʳ����ġ�

## �����ʽ
����ڱ�֤ÿ��ǰ׺��ʳ����������£�Danny ��໹�ܹ��򲢳Ե����ٿ��ǡ�

����ǹ�������û�����ޣ��� Danny ��һֱ����ȥ������� `forever`��


```input1
6 5
2 1 6 3 5 3
1 2 5 3 5

```

```output1
1


```

```input2
6 4
2 1 6 3 5 3
1 2 5 3

```

```output2
forever


```

## ��ʾ
Time limit: 2000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2016

