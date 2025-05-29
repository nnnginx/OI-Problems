## ��Ŀ����
Each of Farmer John's N (1 <= N <= 50,000) cows likes to graze in a certain part of the pasture, which can be thought of as a large one-dimeensional number line. Cow i's favorite grazing range starts at location S\_i and ends at location E\_i (1 <= S\_i < E\_i; S\_i < E\_i <= 100,000,000).

Most folks know the cows are quite selfish; no cow wants to share any of its grazing area with another. Thus, two cows i and j can only graze at the same time if either S\_i >= E\_j or E\_i <= S\_j. FJ would like to know the maximum number of cows that can graze at the same time for a given set of cows and their preferences.

Consider a set of 5 cows with ranges shown below:

```cpp
  ... 1    2    3    4    5    6    7    8    9   10   11   12   13 ...
  ... |----|----|----|----|----|----|----|----|----|----|----|----|----
Cow 1:      <===:===>          :              :              :
Cow 2: <========:==============:==============:=============>:
Cow 3:          :     <====>   :              :              :
Cow 4:          :              :     <========:===>          :
Cow 5:          :              :     <==>     :              :
```
These ranges represent (2, 4), (1, 12), (4, 5), (7, 10), and (7, 8), respectively.

For a solution, the first, third, and fourth (or fifth) cows can all graze at the same time. If the second cow grazed, no other cows could graze. Also, the fourth and fifth cows cannot graze together, so it is impossible for four or more cows to graze.

Լ����N(1��N��50000)ͷţ��Լ���Ĳݵؿ�����Ϊ��һ��ֱ�ߣ�ÿֻţֻϲ����ĳ���ض��ķ�Χ�ڳԲݣ���iͷţϲ��������(Si��Ei)�Բݣ�1��Si<Ei��1,000,000,00.

��ţ�Ƕ�����˽�����ǲ�ϲ����������ţ�����Լ�ϲ���Բݵ��������Լ��Ҫ��֤����

��ͷţ�����Ṳ������ϲ���Բ������������ţi����ţJ��Ҫͬʱ�Բݣ���ôҪ���㣺Si>=Ej����Ei��Sj��Լ����֪����ͬһʱ�̣��������ж���ͷ��ţͬʱ�Բݣ�


## �����ʽ
\* Line 1: A  single integer: N

\* Lines 2..N+1: Line i+1 contains the two space-separated integers: S\_i and E\_i


## �����ʽ
\* Line 1: A single integer representing the maximum number of cows that can graze at once.


```input1
5 
2 4 
1 12 
4 5 
7 10 
7 8 

```

```output1
3 

```

