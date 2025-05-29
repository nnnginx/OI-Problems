## ��Ŀ����
Farmer John has $N$ cows $(2 \le N \le 10^5)$. Each cow has a breed that is either Guernsey or Holstein. As is often the case, the cows are standing in a line, numbered $1 \cdots N$ in this order.

Over the course of the day, each cow writes down a list of cows. Specifically, cow $i$
's list contains the range of cows starting with herself (cow $i$) up to and including cow $E_i(i \le E_i \le N)$.

FJ has recently discovered that each breed of cow has exactly one distinct leader. FJ does not know who the leaders are, but he knows that each leader must have a list that includes all the cows of their breed, or the other breed's leader (or both).

Help FJ count the number of pairs of cows that could be leaders. It is guaranteed that there is at least one possible pair. 

## �����ʽ
The first line contains $N$.

The second line contains a string of length $N$
, with the ith character denoting the breed of the $i$-th cow (G meaning Guernsey and H meaning Holstein). It is guaranteed that there is at least one Guernsey and one Holstein.

The third line contains $E_1 \cdots E_N$. 

## �����ʽ
Output the number of possible pairs of leaders. 

## ��Ŀ����
### ��������

FJ �� $N$ ͷ��ţ��ÿһͷ��ţ��Ʒ���Ǹ����� `G` ���˹̹ `H` �е�һ�֡�

ÿһͷ��ţ����һ���������� $i$ ͷ��ţ�������ϼ�¼�˴ӵ� $i$ ͷ��ţ���� $E_i$ ͷ��ţ��������ţ��

ÿһ����ţ�����ҽ���һλ���쵼�ߡ�������ĳһͷţ $i$��������ܳ�Ϊ���쵼�ߡ���������������������**����һ��**��

- ���¼�������ϰ�������Ʒ�ֵ�������ţ��

- ���¼�������ϼ�¼����һƷ����ţ�ġ��쵼�ߡ���

������ж��ٶ���ţ���ܳ�Ϊ������ţ���쵼�ߣ���֤��������һ�֡�

### ���ݷ�Χ
���� $100\%$ �����ݣ�$1\leq N\leq 2\times 10^5,i\leq E_i\leq N$��

```input1
4
GHHG
2 4 3 4
```

```output1
1
```

```input2
3
GGH
2 3 3
```

```output2
2
```

## ��ʾ
### Explanation for Sample 1

The only valid leader pair is $(1,2)$. Cow $1$'s list contains the other breed's leader (cow $2$). Cow $2$'s list contains all cows of her breed (Holstein).

No other pairs are valid. For example, $(2,4)$
is invalid since cow $4$'s list does not contain the other breed's leader, and it also does not contain all cows of her breed.

### Explanation for Sample 2

There are two valid leader pairs, $(1,3)$ and $(2,3)$.

### Scoring

 - Inputs $3-5$: $N \le 100$  
 - Inputs $6-10$: $N \le 3000$
 - Inputs $11-17$: No additional constraints.

