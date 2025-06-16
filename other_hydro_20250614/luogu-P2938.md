## ��Ŀ����
Despite their innate prudence, the cows took a beating in the home mortgage market and now are trying their hand at stocks. Happily, Bessie is prescient and knows not only today's S (2 <= S <= 50) stock prices but also the future stock prices for a total of D days (2 <= D <= 10).

Given the matrix of current and future stock prices on various days (1 <= PR\_sd <= 1,000) and an initial M (1 <= M <= 200,000) units of money, determine an optimal buying and selling strategy in order to maximize the gain realized by selling stock on the final day. Shares must be purchased in integer multiples, and you need not spend all the money (or any money). It is guaranteed that you will not be able to earn a profit of more than 500,000 units of money.

Consider the example below of a bull (i.e., improving) market, the kind Bessie likes most. In this case, S=2 stocks and D=3 days. The cows have 10 units of money to invest.

| Stock | Today's price | Tomorrow's price |    Two days hence Stock   |
| :---: | :-----------: | :--------------: | :--: |
|  $A$  |      10       |        15        |  15  |
|  $B$  |      13       |        11        |  20  |

If money is to be made, the cows must purchase stock 1 on day 1. Selling stock 1 on day 2 and quickly buying stock 2 yields 4 money in the bank and one share of 2. Selling stock 2 on the final day brings in 20 money for a total of 24 money when the 20 is added to the bank.


## �����ʽ
\* Line 1: Three space-separated integers: S, D, and M

\* Lines 2..S+1: Line s+1 contains the D prices for stock s on days 1..D: PR\_sd


## �����ʽ
\* Line 1: The maximum amount of money possible to have after selling on day D.


## ��Ŀ����
# ��Ŀ����

������ţ����������������Ȼ��ס����Ѻ�Ŵ��г��д��ܴ������������׼���ڹ����������������������ڲ���Ϣ����֪�� $S$ ֻ��Ʊ�ڽ�� $D$ ���ڵļ۸�

������һ��ʼ�����Ｏ�� $M$ ԪǮ����ô����������������׬������Ǯ�أ�������ÿ�����������ֻ��Ʊ��Ҳ���Զ������ͬһֻ��Ʊ�����׵�λ�������������������ޡ���һ��ţ�е����ӣ�

���豴���� $10$ Ԫ���𣬹�Ʊ�۸����£�

|  ��Ʊ | ����ļ۸� | ����ļ۸� | ����ļ۸� |
| :-: | :---: | :---: | :---: |
| $A$ |   $10$  |   $15$  |   $15$  |
| $B$ |   $13$  |   $11$  |   $20$  |

��׬Ǯ�������ǣ��������� $A$ �� $1$ �ţ���������������������� $B$ �� $1$ �ţ��ں������� $B$ �ɣ������������� $24$ Ԫ�ˡ�

# �����ʽ

��һ�У��������� $S,D$ �� $M$��$2\le S\le 50,2\le D\le 10,1\le M\le 200000$��

�ڶ��е��� $S + 1$ �У��� $i + 1$ ���� $D$ ��������$P_{i,1}$ �� $P_{i,D}$����ʾ�� $i$ �ֹ�Ʊ�ڵ�һ�쵽���һ����ۼۣ������� $1\le j\le D$��$1\le P_{i,j}\le 1000$��

# �����ʽ

������������ʾ��ţ���Ի�õ����Ǯ������֤��������ᳬ�� $500000$��

```input1
2 3 10 
10 15 15 
13 11 20 

```

```output1
24 

```

