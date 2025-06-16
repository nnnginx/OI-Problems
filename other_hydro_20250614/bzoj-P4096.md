


## 题目描述
Farmer John has N cows that need to be milked (1 <= N <= 10,000), each of which takes only one unit of time to milk. Being impatient animals, some cows will refuse to be milked if Farmer John waits too long to milk them. More specifically, cow i produces g_i gallons of milk (1 <= g_i <= 1000), but only if she is milked before a deadline at time d_i (1 <= d_i <= 10,000). Time starts at t=0, so at most x total cows can be milked prior to a deadline at time t=x. Please help Farmer John determine the maximum amount of milk that he can obtain if he milks the cows optimally. 
## 输入格式
* Line 1: The value of N. 
* Lines 2..1+N: Line i+1 contains the integers g_i and d_i.
## 输出格式
* Line 1: The maximum number of gallons of milk Farmer John can obtain.

```input1
4
10 3
7 5
8 1
2 1
INPUT DETAILS: There are 4 cows. The first produces 10 gallons of milk if milked by time 3, and so on.

```

```output1
25
OUTPUT DETAILS: Farmer John milks cow 3 first, giving up on cow 4 since she cannot be milked by her deadline due to the conflict with cow 3. Farmer John then milks cows 1 and 2.
```

## 提示
没有写明提示
## 题目来源
Silver


