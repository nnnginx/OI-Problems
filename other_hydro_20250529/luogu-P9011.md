## ��Ŀ����
With the hottest recorded summer ever at Farmer John's farm, he needs a way to cool down his cows. Thus, he decides to invest in some air conditioners.

Farmer John's $N$ cows $(1 \le N \le 20)$ live in a barn that contains a sequence of stalls in a row, numbered $1 \cdots 100$. Cow $i$ occupies a range of these stalls, starting from stall $s_i$ and ending with stall $t_i$. The ranges of stalls occupied by different cows are all disjoint from each-other. Cows have different cooling requirements. Cow $i$ must be cooled by an amount $c_i$, meaning every stall occupied by cow $i$ must have its temperature reduced by at least $c_i$ units.

The barn contains $M$ air conditioners, labeled $1 \cdots M (1 \le M \le 10)$. The $i$-th air conditioner costs $m_i$ units of money to operate $(1 \le m_i \le 1000)$ and cools the range of stalls starting from stall $a_i$ and ending with stall $b_i$. If running, the $i$-th air conditioner reduces the temperature of all the stalls in this range by $p_i (1 \le p_i \le 10^6)$. Ranges of stalls covered by air conditioners may potentially overlap.

Running a farm is no easy business, so FJ has a tight budget. Please determine the minimum amount of money he needs to spend to keep all of his cows comfortable. It is guaranteed that if FJ uses all of his conditioners, then all cows will be comfortable. 

## �����ʽ
The first line of input contains $N$ and $M$.

The next $N$ lines describe cows. The ith of these lines contains $s_i, t_i$, and $c_i$.

The next $M$ lines describe air conditioners. The ith of these lines contains $a_i, b_i, p_i$, and $m_i$.

For every input other than the sample, you can assume that $M=10$. 

## �����ʽ
Output a single integer telling the minimum amount of money FJ needs to spend to operate enough air conditioners to satisfy all his cows (with the conditions listed above). 

## ��Ŀ����
## ��Ŀ����

ũ��Լ���� $N$ ͷ��ţ $(1��N��20)$ ס��һ���Ȳ���Ȳ�����������ţ�������Ϊ $1-100$ �� ��ţ $i$ ռ���˱�� $[s_i,t_i]$ ��ţ���� ��ͬ��ţռ�ݵ�ţ����Χ�ǻ����ཻ�ġ� ��ţ�в�ͬ����ȴҪ����ţ $i$ ռ�õ�ÿ��ţ�����¶ȱ������ٽ��� $c_i$ ��λ��

�Ȳְ��� $M$ ̨�յ������Ϊ $1-M$ $(1\le M\le10)$���� $i$ ̨�յ���Ҫ���� $m_i$ ��λ�Ľ�Ǯ������ $(1\le m_i \le 1000)$ ��������У��� $i$ ̨�յ���ţ�� $[a_i,b_i]$ ����ţ�����¶Ƚ��� $p_i$��$1\le p_i\le10^6��$�� �յ����ǵ�ţ����Χ���ܻ��ص���

�����ũ��Լ���������������ţ����Ҫ���ѵ����ٽ�Ǯ��

## �����ʽ

��һ�������������ֱ�Ϊ $N$ �� $M$��

�� $2$ �� $(N+1)$ �У�ÿ�������������ֱ�Ϊ $s_i$��$t_i$ �� $c_i$ ��

�� $(N+2)$ �� $(M+N+1)$ �У�ÿ���ĸ������� �ֱ�Ϊ $a_i$��$b_i$��$p_i$ �� $m_i$��

## �����ʽ

һ����������ʾ���ٻ��ѵĽ�Ǯ��



## ��ʾ

### �������� 1

һ�ֻ������ٵĿ��ܽ��������ѡ����Щ��ȴ����Ϊ $[2,9]$ ��$[1,2]$ �� $[6,9]$ �Ŀյ����ɱ�Ϊ $ 3+2+5=10$ .

### ���ݷ�Χ

���� $100\%$ �����ݣ�$1 \le N \le 20$�� $1 \le M \le 10$, $ 1 \le a_i, b_i, s_i, t_i \le 100$, $1 \le c_i, p_i \le 10^6$�� $1 \le m_i \le 1000$��

```input1
2 4
1 5 2
7 9 3
2 9 2 3
1 6 2 8
1 2 4 2
6 9 1 5
```

```output1
10
```

## ��ʾ
### Explanation for Sample 1

One possible solution that results in the least amount of money spent is to select those that cool the intervals $[2,9], [1,2]$, and $[6,9]$, for a cost of $3+2+5=10$. 

