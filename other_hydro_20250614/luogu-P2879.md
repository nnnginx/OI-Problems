## ��Ŀ����
FJ's N (1 �� N �� 10,000) cows conveniently indexed 1..N are standing in a line. Each cow has a positive integer height (which is a bit of secret). You are told only the height H (1 �� H �� 1,000,000) of the tallest cow along with the index I of that cow.

FJ has made a list of R (0 �� R �� 10,000) lines of the form "cow 17 sees cow 34". This means that cow 34 is at least as tall as cow 17, and that every cow between 17 and 34 has a height that is strictly smaller than that of cow 17.

For each cow from 1..N, determine its maximum possible height, such that all of the information given is still correct. It is guaranteed that it is possible to satisfy all the constraints.



## �����ʽ
Line 1: Four space-separated integers: N, I, H and R


Lines 2..R+1: Two distinct space-separated integers A and B (1 �� A, B �� N), indicating that cow A can see cow B.


## �����ʽ
Lines 1..N: Line i contains the maximum possible height of cow i.


## ��Ŀ����
**����Ŀ������**

FarmerJohn ��nͷţ�����ǰ�˳���ų�һ�С�FarmerJohn ֻ֪��������ߵ���ţ����ż����ĸ߶ȣ�������ţ�ĸ߶ȶ���δ֪�ġ����� FarmerJohn ������ $R$ ����Ϣ��ÿ����Ϣ������ͷ��ţ����ţ�$a$ �� $b$�������� $b$ ��ţ�ĸ߶�һ�����ڵ��� $a$ ��ţ�ĸ߶ȣ��� $a, b$֮���������ţ�ĸ߶ȶ��� $a$ С������ FarmerJohn �����������Щ��Ϣ���ÿһͷ��ţ�Ŀ��ܵ����ĸ߶ȡ������ݱ�֤�н⣩

**�������ʽ��**

��һ�У��ĸ��Կո�ָ���������$n, i, h, R$��$n$ �� $R$ ��������棻$i$ �� $h$ ��ʾ�� $i$ ͷţ�ĸ߶�Ϊ $h$��������ߵ���ţ��

������ $R$ �У�������ͬ������ $a$ �� $b$��$1 \le a, b \le n$��

**�������ʽ��**

һ�� $n$ �У���ʾÿͷ��ţ�������ܸ߶�.

**�����ݷ�Χ��**

$1 \le n \le 10000$��$1 \le h \le 1000000$��$0 \le R \le 10000$

Translate provided by @��Ƥ

```input1
9 3 5 5
1 3
5 3
4 3
3 7
9 8
```

```output1
5
4
5
3
4
4
5
5
5
```

