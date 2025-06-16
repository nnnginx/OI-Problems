## ��Ŀ����
One sunny day farmer John was kidnapped by evil farmer Marcus's cows. FJ wasn't too concerned about his forced holiday but wanted to make sure that his cows got home safely together.

The cows are spread out in every one of FJ's N (3 <= N <= 200) pastures conveniently numbered 1..N. The barn is located at pasture 1. The farm has an interesting navigation system: at every pasture i there are M (1 <= M <= 200) signs S\_ij (1 <= S\_ij <= N) which one could reference as S\_i1..S\_iM; each sign points the way to a pasture. Sometimes a sign points to a path that leads back to the same

pasture.

Farmer Marcus's cows allow FJ to write a single message to all of his cows. FJ's plan is to write a list of sign numbers such that any cow who follows those instructions will all arrive at the barn when each cow has completed all the instructions.

When a cow starts at a given pasture then she will first follow the path indicated by the first sign number on FJ's list. When she arrives at the second pasture, she looks at the second sign of FJ's list and follows the path marked by that sign. She continues until she exhausts the instruction list, at which point she should be at the barn.

Find a list of instructions containing no more than 5,000,000 sign numbers that will guide every cow, from every pasture, to the barn after all instructions are followed.  It is guaranteed that such a list exists.

Consider a set of three signs in four pastures that direct the cows like these do:

```cpp
** Pasture# ** 
1    2    3    4 
Sign 1   4    4    1    3 
Sign 2   1    3    2    4 
Sign 3   4    2    3    1 
```
The set of instructions below will direct cows to the barn from any of the four pastures:

```cpp
Instruction#   Sign#            Instruction#   Sign# 
1           1                   5           3 
2           2                   6           1 
3           1                   7           3 
4           2 
```
The cow in pasture 1 will read sign #1 at time 1 and be directed to pasture 4.  At time 2, she is in pasture 4 and (per FJ's

instructions) read sign #2 and then be directed to pasture 4. Below is a table that shows the cow's travels:

```cpp
* * * *  Cow in pasture  1  * * * * 
Time    CurrentPasture#    WhichSign     Sign->Nextpasture 
1            1               1                4 
2            4               2                4 (same pasture!) 
3            4               1                3 
4            3               2                2 
5            2               3                2 (same pasture)
6            2               1                4 
7            4               3                1 Barn! 
```
Similarly: Pasture 2's cow visits pastures [2]-4-4-3-2-2-4-1. Pasture 3's cow visits pastures [3]-1-1-4-4-1-4-1.

Pasture 4's cow visits pastures [4]-3-2-4-4-1-4-1.


Given a set of signs, create a set of instructions. 


## �����ʽ
\* Line 1: Two space separated integers: N and M

\* Lines 2..M+1: Line i+1 describes the contents of each pasture's N signs with N integers: S\_1i..S\_Ni


## �����ʽ
\* Lines 1..?: The sign numbers the cows should follow, one per line.


## ��Ŀ����
### ��Ŀ����

����һ�� $n(3\leq n\leq 200)$ �����ͼ��ÿ���㶼ǡ���� $m(1\leq m\leq 200)$ �����ߣ��� $i$ ����ĵ� $j$ ������ָ�� $a_{i,j}$��

��������ͼ��ÿ���㶼��һͷţ��ÿ������Ա���һ���� $x(1\leq x\leq m)$�����ʹ��ÿһͷţ���ŵ�ǰ���ڵĵ�ĵ� $x$ ������һ��������ǰ�ڵ� $u$ ��ţ�ƶ����� $a_{u,x}$����

����Ҫ���������� $5\times 10^6$ ��ָ�ʹ�������е�ָ��ִ��������е�ţ���ڱ��Ϊ $1$ �ĵ��ϡ�

### �����ʽ

��һ���������� $n,m$��

������ $m$ ��ÿ�� $n$ ���������� $i$ �еĵ� $j$ �������� $a_{j,i}$��

### �����ʽ

�ڵ� $i$ ������㷢���ĵ� $i$ ��ָ�

```input1
4 3 
4 4 1 3 
1 3 2 4 
4 2 3 1 

```

```output1
1 
2 
1 
2 
3 
1 
3 

```

