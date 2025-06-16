## ��Ŀ����
A factory receives $n$ orders at the beginning of day $1$. The $i$-th order can be described as two integers $a_i$ and $b_i$, indicating that at the end of day $a_i$, the factory needs to deliver $b_i$ products to the customer.

Given that the factory can produce $k$ products each day, and at the beginning of day $1$ the factory has no product in stock, can the factory complete all orders?

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \le T \le 100$) indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $k$ ($1 \le n \le 100$, $1 \le k \le 10^9$) indicating the number of orders and the number of products the factory can produce each day.

For the following $n$ lines, the $i$-th line contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 10^9$) indicating that the $i$-th order require the factory to deliver $b_i$ products at the end of day $a_i$.

## �����ʽ
For each test case output one line. If the factory can complete all orders output $\texttt{Yes}$, otherwise output $\texttt{No}$.

## ��Ŀ����
**����Ŀ������**

ĳ�����ڵ� $1$ �쿪��֮ǰ�յ��� $n$ �ʶ������� $i$ �ʶ����������������� $a_i$ �� $b_i$ ��������ʾ������Ҫ�ڵ� $a_i$ �����ʱ���� $b_i$ �����

��֪����ÿ�������� $k$ ������ҵ� $1$ �쿪��֮ǰû���κδ�����ʸù����ܷ�������ж�����

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$��$1 \le T \le 100$����ʾ������������������ÿ��������ݣ�

��һ�������������� $n$ �� $k$��$1 \le n \le 100$��$1 \le k \le 10^9$����ʾ���������Լ�����ÿ���������Ļ���������

���ڽ����� $n$ �У��� $i$ �������������� $a_i$ �� $b_i$��$1 \le a_i, b_i \le 10^9$����ʾ�� $i$ �ʶ���Ҫ���ڵ� $a_i$ �����ʱ���� $b_i$ �����

**�������ʽ��**

ÿ���������һ�С���������������ж������ $\texttt{Yes}$��������� $\texttt{No}$��

**���������͡�**

���ڵ�һ���������ݣ�����ÿ�������� $5$ �����
-  �ڵ� $1$ �����ʱ���������� $5$ �����������ɵ� $2$ �ʶ����������󣬹���ʣ�� $2$ �����
-  �ڵ� $6$ �����ʱ�������ֶ������� $25$ ��������� $27$ �����������ɵ� $1$ �͵� $3$ �ʶ����������󣬹���ʣ�� $0$ �����
- �ڵ� $8$ �����ʱ�������ֶ������� $10$ ��������� $10$ �����������ɵ� $4$ �ʶ����������󣬹���ʣ�� $9$ �����

���ڵڶ����������ݣ�����ÿ�������� $100$ �����
- �ڵ� $3$ �����ʱ���������� $300$ �����������ɵ� $1$ �ʶ����������󣬹���ʣ�� $100$ �����
- �ڵ� $4$ �����ʱ�������ֶ������� $100$ ��������� $200$ ������޷���ɵ� $2$ �ʶ�����

```input1
2
4 5
6 12
1 3
6 15
8 1
3 100
3 200
4 300
6 100
```

```output1
Yes
No
```

## ��ʾ
For the first sample test case, the factory can produce $5$ products each day.

- At the end of day $1$, there are $5$ products in stock so the factory can complete the $2$-nd order. After delivery, there are $2$ products left in stock.
- At the end of day $6$, the factory produces $25$ more products. There are $27$ products in stock so the factory can complete the $1$-st and the $3$-rd order. After delivery, there are $0$ products left in stock.
- At the end of day $8$, the factory produces $10$ more products. There are $10$ products in stock so the factory can complete the $4$-th order. After delivery, there are $9$ products left in stock.

For the second sample test case, the factory can produce $100$ products each day.

- At the end of day $3$, there are $300$ products in stock and the factory can complete the $1$-st order. After delivery, there are $100$ products left in stock.
- At the end of day $4$, the factory produces $100$ more products. There are only $200$ products in stock so the factory cannot complete the $2$-nd order.

