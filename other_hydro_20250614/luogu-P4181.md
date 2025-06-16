## ��Ŀ����
Farmer John realizes that the income he receives from milk production is insufficient to fund the growth of his farm, so to earn some extra money, he launches a cow-rental service, which he calls "USACOW" (pronounced "Use-a-cow").

Farmer John has $N$ cows ($1 \leq N \leq 100,000$), each capable of producing some amount of milk every day. The $M$ stores near FJ's farm ($1 \leq M \leq 100,000$) each offer to buy a certain amount of milk at a certain price. Moreover, Farmer John's $R$ ($1 \leq R \leq 100,000$) neighboring farmers are each interested in renting a cow at a certain price.


Farmer John has to choose whether each cow should be milked or rented to a nearby farmer. Help him find the maximum amount of money he can make per day.


## �����ʽ
The first line in the input contains $N$, $M$, and $R$. The next $N$ lines each contain an integer $c_i$ ($1 \leq c_i \leq 1,000,000$), indicating that Farmer John's $i$th cow can produce $c_i$ gallons of milk every day. The next $M$ lines each contain two integers $q_i$ and $p_i$ ($1 \leq q_i, p_i \leq 1,000,000$), indicating that the $i$th store is willing to buy up to $q_i$ gallons of milk for $p_i$ cents per gallon. Keep in mind that Farmer John can sell any amount of milk between zero and $q_i$ gallons to a given store. The next $R$ lines each contain an integer $r_i$ ($1 \leq r_i \leq 1,000,000$), indicating that one of Farmer John's neighbors wants to rent a cow for $r_i$ cents per day.


## �����ʽ
The output should consist of one line containing the maximum profit Farmer John can make per day by milking or renting out each of his cows. Note that the output might be too large to fit into a standard 32-bit integer, so you may need to use a larger integer type like a "long long" in C/C++.


## ��Ŀ����
### ��Ŀ����

Farmer John ��ʶ��ţ�����������벻����֧��ũ������չ�����Ϊ��׬ȡ�������룬���Ƴ���һ����ţ���޷��񣬳�Ϊ��USACOW��������Ϊ��Use-a-cow������

Farmer John �� $N$ ͷ��ţ��$1 \leq N \leq 100,000$����ÿͷ��ţÿ���������һ������ţ�̡������� $M$ ���̵꣨$1 \leq M \leq 100,000$��ÿ�Ҷ�Ը����һ���۸���һ������ţ�̡����⣬Farmer John �� $R$ ���ھӣ�$1 \leq R \leq 100,000$��ÿ�Ҷ�Ը����һ���۸�����һͷ��ţ��

Farmer John ��Ҫ����ÿͷ��ţ�����ڲ��̻������������ũ�������������ÿ�����׬ȡ������

### �����ʽ

����ĵ�һ�а��� $N$��$M$ �� $R$���������� $N$ ��ÿ�а���һ������ $c_i$��$1 \leq c_i \leq 1,000,000$������ʾ Farmer John �ĵ� $i$ ͷ��ţÿ��������� $c_i$ ����ţ�̡��������� $M$ ��ÿ�а����������� $q_i$ �� $p_i$��$1 \leq q_i, p_i \leq 1,000,000$������ʾ�� $i$ ���̵�Ը����ÿ���� $p_i$ ���ֵļ۸������ $q_i$ ����ţ�̡���ע�⣬Farmer John ������ÿ���̵��������������ţ�̣���Χ�� $0$ �� $q_i$ ���ء��������� $R$ ��ÿ�а���һ������ $r_i$��$1 \leq r_i \leq 1,000,000$������ʾ Farmer John ��һ���ھ�Ը����ÿ�� $r_i$ ���ֵļ۸�����һͷ��ţ��

### �����ʽ

���Ӧ����һ�У���ʾ Farmer John ͨ�����̻�������ţÿ����Ի�õ����������ע�⣬������ܳ�����׼ 32 λ�����ķ�Χ����˿�����Ҫʹ�ø�����������ͣ����� C/C++ �е� `long long`��

### ��ʾ

Farmer John Ӧ������ţ #1 �� #4 ���̣�ÿ������ $13$ ����ţ�̡���Ӧ����ȫ���� $10$ ���صĶ�����׬ȡ $250$ ���֣�����ÿ���� $15$ ���ֵļ۸����ʣ��� $3$ ���أ��ܹ�׬ȡ $295$ ���ֵ�ţ������

Ȼ����Ӧ�ý�������ͷ��ţ�ֱ��� $250$��$80$ �� $100$ ���ֵļ۸������׬ȡ����� $430$ ���֡�����Ӧ�ú��� $40$ ���ֵ��������󡣣���������ÿ���������Ϊ $725$ ���֡�

```input1
5 3 4
6
2
4
7
1
10 25
2 10
15 15
250
80
100
40
```

```output1
725

```

## ��ʾ
Farmer John should milk cows #1 and #4, to produce 13 gallons of milk. He should completely fill the order for 10 gallons, earning 250 cents, and sell the remaining three gallons at 15 cents each, for a total of 295 cents of milk profits.


Then, he should rent out the other three cows for 250, 80, and 100 cents, to earn 430 more cents. (He should leave the request for a 40-cent rental unfilled.) This is a total of 725 cents of daily profit.


