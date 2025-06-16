## ��Ŀ����
Little Vasya is playing a new game named "Dwarf Tower". In this game there are $n$ different items, which you can put on your dwarf character. Items are numbered from $1$ to $n$ . Vasya wants to get the item with number $1$ .

There are two ways to obtain an item:

You can buy an item. The i-th item costs $c_i$ money.

You can craft an item. This game supports only $m$ types of crafting. To craft an item, you give two particular different items and get another one as a result.

Help Vasya to spend the least amount of money to get the item number $1$ .


## �����ʽ
The first line contains two integers $n$ and $m (1 \le n \le 10000 , 0 \le m \le 100000) -$ the number of different items and the number of crafting types.

The second line contains $n$ integers $c_i -$ values of the items $(0 \le c_i \le 10^9)$ .

The following $m$ lines describe crafting types, each line contains three distinct integers $a_i, x_i, y_i$ -- $a_i$ is the item that can be crafted from items $x_i$ and $y_i (1 \le  a_i, x_i, y_i \le n , a_i \ne x_i, x_i \ne y_i, y_i \ne a_i)$.

## �����ʽ

Print a single integer -- the least amount of money to spend. 

## ��Ŀ����
### ��Ŀ����
СVasya ����һ������Ϸ���� Dwarf Tower���������Ϸ���� $n$ ����ͬ���������İ��ˡ������ $1$ �� $n$ ���б�š�Vasya ��Ҫ��ñ��Ϊ $1$ �����

���������ַ������һ�����

1. ������������� $i$ ����Ʒ���� $c_i$ Ԫ��

1. �㻹�����������������Ϸ֧�� $m$ ������������Ҫ����һ���������Ҫ���������ض������

��� Vasya ������Ҫ����Ǯ�����һ�����

### �����ʽ
��һ�������������� $n$ , $m$ $(1 \le n \le 10000 , 0 \le m \le 100000) $ ������ $n$ ��������� $m$ ������������

�ڶ������� $n$ ���������� $i$ ���������� $c_i$ $(0 \le c_i \le 10^9)$ ��

������ $m$ ��ÿ������������ $a_i, x_i, y_i$ $(1 \le a_i, x_i, y_i \le n , a_i \ne x_i, x_i \ne y_i, y_i \ne a_i)$ ��$a_i$ ���� $a_i$ ���Ա� $x_i$ �� $y_i$ ������

### �����ʽ
һ������������ Vasya ������Ҫ����Ǯ�����һ�����

```input1
5 3
5 0 1 2 5
5 2 3
4 2 3
1 4 5

```

```output1
2

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



