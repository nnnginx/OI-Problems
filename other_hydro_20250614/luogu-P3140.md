## ��Ŀ����
After the last debacle involving Farmer John's circular barn, one would think he had learned his lesson about non-traditional architecture.  However, he thinks he can still make his circular barn (from the preceding problem) function properly by allowing multiple cows into each room.  To recap, the barn consists of a ring of $n$ rooms,  numbered clockwise from $1 \ldots n$ around the perimeter of the barn ($3 \leq n \leq 100$).  Each room has doors to its two neighboring rooms, and also a door opening to the exterior of the barn.

Farmer John wants exactly $r_i$ cows to end up in room $i$ ($1 \leq r_i \leq 1,000,000$). To herd the cows into the barn in an orderly fashion, he plans to unlock $k$ exterior doors ($1 \leq k \leq 7$), allowing the cows to enter through only those doors. Each cow then walks clockwise through the rooms until she reaches a suitable destination.  Farmer John wants to unlock the exterior doors that will cause his cows to collectively walk a minimum total amount of distance after entering the barn (they can initially line up however they like outside the $k$ unlocked doors; this does not contribute to the total distance in question).  Please determine the minimum total distance his cows will need to walk, if he chooses the best $k$ such doors to unlock.

## �����ʽ
The first line of input contains $n$ and $k$.  Each of the remaining $n$ lines contain $r_1 \ldots r_n$.


## �����ʽ
Please write out the minimum amount of distance the cows need to travel.


## ��Ŀ����
### ��Ŀ����

����һ���漰 Farmer John ��Բ�ιȲֵĲҰ�֮�����ǿ��ܻ���Ϊ���Ѿ���ȡ�˹��ڷǴ�ͳ�����Ľ�ѵ��Ȼ��������Ϊͨ������ÿ�䷿������ͷ��ţ����Ȼ���������Ǹ�Բ�ιȲ֣�����֮ǰ�����⣩�����������ع�һ�£��Ȳ��� $n$ ��������ɣ���Щ����˳ʱ����Ϊ $1 \ldots n$��Χ�ƹȲֵ��ܱ����У�$3 \leq n \leq 100$����ÿ�����䶼��ͨ���������ڷ�����ţ�����һ����ͨ��Ȳֵ��ⲿ��

Farmer John ϣ��������ǡ�� $r_i$ ͷ��ţ���뷿�� $i$��$1 \leq r_i \leq 1,000,000$����Ϊ������ţ����ؽ���Ȳ֣����ƻ����� $k$ ���ⲿ�ţ�$1 \leq k \leq 7$����ֻ������ţͨ����Щ�Ž��롣ÿͷ��ţ���˳ʱ�봩�����䣬ֱ��������ʵ�Ŀ�ĵء�Farmer John ϣ��������Щ����������ţ�ڽ���Ȳֺ��ܹ����ߵľ�����С���ⲿ�ţ�������������� $k$ �Ƚ����������������У��ⲻ������ܾ��룩����ȷ�������ѡ����ѵ� $k$ ���Ž�����������ţ��Ҫ���ߵ���С�ܾ��롣

### �����ʽ

����ĵ�һ�а��� $n$ �� $k$���������� $n$ ��ÿ�а��� $r_1 \ldots r_n$��

### �����ʽ

�������ţ��Ҫ���ߵ���С���롣

### ˵��/��ʾ

Farmer John ���Խ����� 2 ���� 5��11 ͷ��ţ���� 2 ���룬�ܹ����� 8 �ľ��뵽�﷿�� 2��3 �� 4��10 ͷ��ţ���� 5 ���룬�ܹ����� 6 �ľ��뵽�﷿�� 5��6 �� 1��

```input1
6 2
2
5
4
2
6
2
```

```output1
14
```

## ��ʾ
Farmer John can unlock doors 2 and 5.  11 cows enter at door 2 and walk a total distance of 8 to get to rooms 2, 3, and 4.  10 cows enter at door 5 and walk a total distance of 6 to get to rooms 5, 6 and 1.


