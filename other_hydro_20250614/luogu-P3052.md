## ��Ŀ����
A little known fact about Bessie and friends is that they love stair climbing races.  A better known fact is that cows really don't like going down stairs.  So after the cows finish racing to the top of their favorite skyscraper, they had a problem.  Refusing to climb back down using the stairs, the cows are forced to use the elevator in order to get back to the ground floor.

The elevator has a maximum weight capacity of W (1 <= W <= 100,000,000) pounds and cow i weighs C\_i (1 <= C\_i <= W) pounds.  Please help Bessie figure out how to get all the N (1 <= N <= 18) of the cows to the ground floor using the least number of elevator rides.  The sum of the weights of the cows on each elevator ride must be no larger than W.


## �����ʽ
\* Line 1: N and W separated by a space.

\* Lines 2..1+N: Line i+1 contains the integer C\_i, giving the weight of one of the cows.


## �����ʽ
\* A single integer, R, indicating the minimum number of elevator rides needed.

one of the R trips down the elevator.  


## ��Ŀ����
���� $n$ ����Ʒ�����Ϊ $w _ 1, w _ 2, \cdots, w _ n$���ְ���ֳ������飬Ҫ��ÿ�������С�ڵ��� $W$������С����������

$n\le 18,1\le c_i\le W\le 10^8$��

```input1
4 10 
5 
6 
3 
7 

```

```output1
3 
```

## ��ʾ
There are four cows weighing 5, 6, 3, and 7 pounds.  The elevator has a maximum weight capacity of 10 pounds.


We can put the cow weighing 3 on the same elevator as any other cow but the other three cows are too heavy to be combined.  For the solution above, elevator ride 1 involves cow #1 and #3, elevator ride 2 involves cow #2, and elevator ride 3 involves cow #4.  Several other solutions are possible for this input.


