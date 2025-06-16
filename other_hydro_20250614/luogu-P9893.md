## ��Ŀ����
DreamGrid and BaoBao are playing a game.  There are $n$ soldiers in the game, numbered from $1$ to $n$. The $i$-th soldier has a power value of $a_i$. DreamGrid and BaoBao are going to divide the soldiers into several teams according to the rules below:

- A team must consist of 1 or 2 soldiers.
- Every soldier must belong to exactly 1 team.
- If a team consists of two soldiers (let's say they are the $i$-th and the $j$-th soldier), there must be $|i - j| = 1$.

The power value of a team is defined as the sum of the team members' power values. For the sake of fairness, they want to minimize the difference between the maximum team power value and the minimum team power value after the division. You are asked to find the minimum difference.



## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($1 \le n \le 10^5$), indicating the number of soldiers.

The second line contains $n$ integers $a_1, a_2, ... , a_n$ ($-10^9 \le a_i \le 10^9$), where $a_i$ indicates the power value of the $i$-th soldier.

It's guaranteed that the sum of $n$ in all test cases will not exceed $10^6$.


## �����ʽ
For each test case output one line containing one integer, indicating the minimum difference between the maximum team power value and the minimum team power value.


## ��Ŀ����
**DreamGrid** �� **BaoBao** ������Ϸ����Ϸ���� $n$ ��ʿ�������Ϊ $1\sim n$���� $i$ ��ʿ����Ȩ��ֵΪ $a_i$��**DreamGrid** �� **BaoBao** ���������¹���ʿ���ֳɼ���С��:

- һ����������� $1$ �� $2$ ��ʿ����ɡ�

- ÿ��ʿ������ֻ����һ�����顣

- ���һ���Ŷ�������ʿ�� $i,j$ ��ɣ�������� $|i - j| = 1$��

�Ŷӵ�Ȩ��ֵ������Ϊ����ʿ��Ȩ��ֵ���ܺ͡�

Ϊ�˹�ƽ���������ϣ����С���������**����Ŷ�����ֵ**��**��С�Ŷ�����ֵ**֮���**��ֵ**���㱻Ҫ���ҳ���С�Ĳ�ֵ��

�ж�⡣

$1\leq n\leq 10 ^ 5$��$|a_i|\leq 10 ^ 9$��$\sum n\leq 10 ^ 6$��

```input1
3
5
-1 4 2 1 1
4
1 3 2 4
1
7
```

```output1
1
2
0
```

## ��ʾ
We now explain the first sample test case. All possible divisions are listed below.

| Division | Difference | Division | Difference |
| :-: | :-: | :-: | :-:|
|[-1], [4], [2], [1], [1] | 4 - (-1) = 5| [-1, 4], [2], [1], [1] | 3 - 1 = 2 |
| [-1], [4], [2], [1, 1] | 4 - (-1) = 5 | [-1], [4, 2], [1, 1] | 6 - (-1) = 7 |
| [-1], [4], [2, 1], [1] | 4 - (-1) = 5 |  [-1, 4], [2], [1, 1] | 3 - 2 = 1 |
| [-1], [4, 2], [1], [1] | 6 - (-1) = 7 | [-1, 4], [2, 1], [1] | 3 - 1 = 2 |


So the answer is $\min(5, 5, 5, 7, 2, 7, 1, 2) = 1$.

