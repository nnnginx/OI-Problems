## ��Ŀ����
Define the ''digit product'' $f(x)$ of a positive integer $x$ as the product of all its digits. For example, $f(1234) = 1 \times 2 \times 3 \times 4 = 24$, and $f(100) = 1 \times 0 \times 0 = 0$.

Given two integers $l$ and $r$, please calculate the following value:
$$(\prod_{i=l}^r f(i)) \mod (10^9+7)$$ 
In case that you don't know what $\prod$ represents, the above expression is the same as 
$$(f(l) \times f(l+1) \times \dots \times f(r)) \mod (10^9+7)$$


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ (about $10^5$), indicating the number of test cases. For each test case:

The first and only line contains two integers $l$ and $r$ ($1 \le l \le r \le 10^9$), indicating the given two integers. The integers are given without leading zeros.


## �����ʽ
For each test case output one line containing one integer indicating the answer.

## ��Ŀ����
**����Ŀ������**

���������� $x$ �� "���ֳ˻�" $f(x)$ Ϊ���������ֵĳ˻������磬$f(1234) = 1 \times 2 \times 3 \times 4 = 24$��$f(100) = 1 \times 0 \times 0 = 0$��

������������ $l$ �� $r$�����������ֵ��
$$(\prod_{i=l}^r f(i)) \mod (10^9+7)$$ 
����㲻֪�� $\prod$ ��ʾʲô���������ʽ��ͬ�� 
$$(f(l) \times f(l+1) \times \dots \times f(r)) \mod (10^9+7)$$

**�������ʽ��**

�ж����������������ĵ�һ�а���һ������ $T$����Լ $10^5$������ʾ��������������������ÿ������������

��һ����Ψһһ�а����������� $l$ �� $r$��$1 \le l \le r \le 10^9$������ʾ������������������Щ����û��ǰ���㡣

**�������ʽ��**

����ÿ���������������һ�У�����һ����������ʾ�𰸡�

**���������͡�**

���ڵ�һ�������������������� $9! \mod (10^9+7) = 362880$��

���ڵڶ��������������������� $(f(97) \times f(98) \times f(99)) \mod (10^9+7) = (9 \times 7 \times 9 \times 8 \times 9 \times 9) \mod (10^9+7) = 367416$��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
2
1 9
97 99

```

```output1
362880
367416

```

## ��ʾ
For the first sample test case, the answer is $9! \mod (10^9+7) = 362880$.

For the second sample test case, the answer is $(f(97) \times f(98) \times f(99)) \mod (10^9+7) = (9 \times 7 \times 9 \times 8 \times 9 \times 9) \mod (10^9+7) = 367416$.


