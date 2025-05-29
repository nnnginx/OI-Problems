## ��Ŀ����

Just like every fall��the organizers of the Southwestern Europe Dice Simulation Contest are busy again this year��In this edition you have to simulate a 3-sided die that outputs each of three possible outcomes ��which will be denoted by $1,2$ and $3$�� with a given probability��using three dice in a given set��The simulation is performed this way��you choose one of the given dice at random��roll it��and report its outcome��You are free to choose the probabilities of rolling each of the given dice��as long as each probability is strictly greater than zero��Before distributing the materials to the contestants��the organizers have to verify that it is actually possible to solve this task��

For example��in the first test case of the sample input you have to simulate a die that yields outcome $1,2$ and $3$ with probabilities��and��We give you three dice��and in this case the $i$-th of them always yields outcome $i$��for each $i = 1,2,3$��Then it is possible to simulate the given die in the following fashion��roll the first die with probability��the second one with probability and the last one with probability��

һ�������� $3$ ���棬$3$ ���棨$A,B,C$ �棩�Ϸֱ��� $3$ �����֡��ڱ����У��ȸ����� $3$ �����ӣ�ÿ�����Ӹ��� $3$ ��������֡����Ǳ�֤����ÿ�����ӣ�$3$ ��������ֺ�Ϊ $1 \times 10^4$��֮���ٸ���һ������ϣ���õ��� $A,B,C$ ��Ľ����Ȼ��ϣ����� $3$ �����ӷ�����ʣ� ��һ�����ӷ������ $p_1$���ڶ��� $p_2$�������� $p_3$�����㣺

1. $p_1 + p_2 + p_3 = 1$

2. $3$ �����ӵ�ÿ����������͵��ڸ������Ǹ���������ĺ�

���磬����1�У�

```
0 0 10000

0 10000 0

10000 0 0
```

����1��$A(0)$��$B(0)$��$C(10000)$��

����2��$A(0)$��$B(10000)$��$C(0)$��

����3��$A(10000)$��$B(0)$��$C(0)$��

Ŀ�꣺$A(3000)$��$B(4000)$��$C(3000)$��

�����ҿ��Է��� $p_1={3} \over {10}$��$p_2={4} \over {10}$��$p_3={3} \over {10}$��

����

$A$ ������: $p_1 \times 0 + p_2 \times 0 + p_3 \times 10000 = 3000$

$B$ ������: $p_1 \times 0 + p_2 \times 10000 + p_3 \times 0 = 4000$

$C$ ������: $p_1 \times 10000 + p_2 \times 0 + p_3 \times 0 = 3000$

�ڱ����У���֤������ $3$ �����Եĺ;�Ϊ $10000$��

## �����ʽ

**�����ж�������**

The input consists of several test cases��separated by single blank lines��Each test case consists of four lines��

the first three of them describe the three dice you are given and the last one describes the die you have to simulate��

Each of the four lines contains $3$ space-separated integers between $0$ and $10000$ inclusive��These numbers will add up to $10000$��and represent $10000$ times the probability that rolling the die described in that line yields outcome $1��2$ and $3$��respectively��

The test cases will finish with a line containing only the number zero repeated three times ��also preceded with a blank line����

����������ݣ�ÿ�����ݸ��� $3$ �����ӵ� $A��B��C$ ��ĵ�����Ȼ�����һ�������Ľ����

��֤������ $3$ �����Եĺ;�Ϊ $10000$��

������� $3$ �� $0$����ô���ʾ���ݽ���

## �����ʽ

For each case��your program should output a line with the word `YES` if it is feasible to produce the desired die from the given ones��and `NO` otherwise��
�������������ԣ�������Է��� $p_1,p_2,p_3$ ������������������� `YES` ������� `NO`��

```input1
0 0 10000
0 10000 0
10000 0 0
3000 4000 3000
0 0 10000
0 10000 0
3000 4000 3000
10000 0 0
0 0 0
```

```output1
YES
NO
```

## ��Ŀ��Դ

��л AekdyCoin