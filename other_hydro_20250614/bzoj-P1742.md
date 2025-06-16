## ��Ŀ����

John ����һֻ�� Joseph ����ţ��һ����ȥ��ţ������һ���ǳ�����һƬ�أ�����Ϊ $l$�������� $n$ ��ط�����ïʢ�Ĳݡ����ǿ�����Ϊ�ݵ���һ�������ϵ�һЩ�㡣Joseph ������Щ�ݷǳ��˷ܣ����������ȫ���Թ⡣��������ʼ�������ߣ��Բݡ�John �� Joseph ��ʼ��ʱ��վ�� $p$ λ�á�Joseph ���ƶ��ٶ���һ����λʱ��һ����λ���롣���ҵ��ǣ��������ʱ�䲻�ԣ��ͻḯ�ܡ����Ƕ���һ�Ѳݵĸ���ֵ�Ǵ� Joseph ��ʼ�Բݵ��Ե���Ѳݵ���ʱ�䡣Joseph �ɲ����̫���ܵĲݣ����� John ��������һ��·�ߣ�ʹ�����������еĲݺ��ܸ���ֵ��С��John ����ѧ���ã�����֪���������������ܰ���ô��

## �����ʽ

* Line $1$: Two space-separated integers: $n$ and $l$.
* Lines $2\dots n+1$: Each line contains a single integer giving the position $p$ of a clump.

## �����ʽ

* Line $1$: A single integer: the minimum total staleness Bessie can achieve while eating all the clumps.

```input1
4 10
1
9
11
19
```
```output1
44
```

## ��������

INPUT DETAILS:

Four clumps: at $1,9,11$, and $19$. Bessie starts at location $10$.

OUTPUT DETAILS:

Bessie can follow this route:  

* start at position $10$ at time $0$.
* move to position $9$, arriving at time $1$.
* move to position $11$, arriving at time $3$.
* move to position $19$, arriving at time $11$.
* move to position $1$, arriving at time $29$.

giving her a total staleness of $1+3+11+29 = 44$. There are other routes with the same total staleness, but no route with a smaller one.

## ���ݷ�Χ

�����������ݣ�$n\le 10^3$��$1 \le  p \le  10^6$��
