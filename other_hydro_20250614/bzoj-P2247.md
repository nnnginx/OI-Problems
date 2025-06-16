

## ��Ŀ����
> In the downtown of Bucharest there is a very big bank with a very big vault. Inside the vault there are $n$ very big boxes numbered from $1\sim n$. Inside the box with number $k$ there are $k$ very big diamonds, each of weight $W_k$ and cost $C_k$. 

> John and Brus are inside the vault at the moment. They would like to steal everything, but unfortunately they are able to carry diamonds with the total weight not exceeding $m$. 

> Your task is to help John and Brus to choose diamonds with the total weight less than or equal to $m$ and the maximal possible total cost.

## ���ķ���

�� Bucharest �е���������һ���ܴ�����У����еĽ�����б��Ϊ $1\sim n$ �� $n$ �ֺ��ӣ��� $k$ ���������� $k$ ������Ϊ $w_k$����ֵΪ $c_k$ ����ʯ��

John �� Brus ���ڽ�������ԣ����Ǳ������������ʯ����ϧ���ǵı�������ֻ�� $m$�����仰˵���� $S$ Ϊ���Ǵ��ߵ���ʯ��ż��ϣ���ô $S$ ������

$$
\sum_{k\in S} w_k \le m
$$

����Ҫ���� John �� Brus��ʹ����������������£����

$$
\sum_{k\in S} c_k
$$

## �����ʽ
>The first line contains single integer $T$ �C the number of test cases. Each test case starts with a line containing two integers $n$ and $m$ separated by a single space. The next line contains $n$ integers $w_k$ separated by single spaces. The following line contains $n$ integers $c_k$ separated by single spaces.

��һ��һ������ $T$����ʾ����������

����ÿ�����ݣ���һ�а������������� $n,m$��

������һ�� $n$ ������������ $i$ ��������ʾ $w_i$��

������һ�� $n$ ������������ $i$ ��������ʾ $c_i$��
## �����ʽ
>For each test case print a single line containing the maximal possible total cost of diamonds.

��ÿ�����ݣ������Ӧ������ֵ��

```input1
2 
2 4 
3 2 
5 3 
3 100 
4 7 1 
5 9 2

```
```output1
6 
29

```

## ��ʾ
$1\le T\le 74,1\le n\le 15,1\le w_i,c_i,m\le 10^9$

## ��Ŀ��Դ
Seerc2009


