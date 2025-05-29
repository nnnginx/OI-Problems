## ��Ŀ����
A railroad siding consists of two (dead-end) sidetracks 1 and 2.

The siding is entered by track A, and left by track B (see figure below).

There are ![](http://main.edu.pl/images/OI17/kol-en-tex.1.png) cars on track A, numbered from ![](http://main.edu.pl/images/OI17/kol-en-tex.2.png) to ![](http://main.edu.pl/images/OI17/kol-en-tex.3.png).

They are arranged in such a way that they enter the siding in the order    ![](http://main.edu.pl/images/OI17/kol-en-tex.4.png).

The cars are to be transferred to the siding, so that they leave it by track B    in the order ![](http://main.edu.pl/images/OI17/kol-en-tex.5.png).

Each car is to be transferred once from track A to one of the sidetracks 1 or 2,    and later (possibly after some transfers of the remaining cars) once from that    sidetrack to the track B.

The sidetracks are long enough to store even the longest trains, so there is    no need to worry about their capacity.

## �����ʽ
The first line of the standard input holds one integer ![](http://main.edu.pl/images/OI17/kol-en-tex.6.png) (![](http://main.edu.pl/images/OI17/kol-en-tex.7.png))      that denotes the number of cars for transfer.

The second line stores the numbers ![](http://main.edu.pl/images/OI17/kol-en-tex.8.png) that are a permutation of ![](http://main.edu.pl/images/OI17/kol-en-tex.9.png)      (i.e., each ![](http://main.edu.pl/images/OI17/kol-en-tex.10.png) belongs to ![](http://main.edu.pl/images/OI17/kol-en-tex.11.png), and all these numbers are unique),      separated by single spaces.


## �����ʽ
The first line of the standard output should contain the word TAK      (yes in Polish) if there is a way of transferring the cars so that they      enter track B in the order ![](http://main.edu.pl/images/OI17/kol-en-tex.12.png), or the word NIE      (no in Polish) if it is impossible.

If the answer is TAK, the second line should give, separated by      single spaces, the numbers of sidetracks (1 or 2) to which successive cars      ![](http://main.edu.pl/images/OI17/kol-en-tex.13.png) are moved in a correct transfer.

If there are several ways of making the transfer, choose one arbitrarily.


## ��Ŀ����
### ��Ŀ����

**���� POI 2010 Stage 1.��[Kolej](https://szkopul.edu.pl/problemset/problem/TJVrS_hRC8W5Q6ZBW6mETAIm/site/?key=statement)��**

һ����·������������ $1$ �� $2$ ������� $A$ ���룬�ұ��� $B$ ��ȥ������ͼ��ʾ����  

![](https://cdn.luogu.com.cn/upload/image_hosting/bdq72qy0.png)

�� $n$ ��������ͨ�� $A$ �ϣ����Ϊ $1$ �� $n$ �����ǰ��� $a_1,a_2,\cdots ,a_n$ ��˳�������ߣ���Ҫ���� $1,2,\cdots ,n$ ��˳���ͨ�� $B$ ��ȥ��    
���ǿ��Դ� $A$ �� $1$ �� $2$ ��Ȼ�󾭹�һϵ��ת�ƴ� $B$ ��ȥ�����ÿ����������⣩�����Ƿ��ܹ�������������ԣ����ҳ�һ�ַ�����

### �����ʽ

��һ��һ�������� $n$ ��  
�ڶ��� $n$ ���ո������������ $a_1,a_2,\cdots a_n$ ��

### �����ʽ

��һ��һ���ַ���������ܹ���������� ```TAK``` ��������� ```NIE``` ��  
�����������ڶ��� $n$ ���ո����������������ʾÿ���������Ĳ��߱�š�  
����ж�⣬�������һ�֡�

���������� [LibreOJ](https://loj.ac/p/2448)��

```input1
4
1 3 4 2
```

```output1
TAK
1 1 2 1
```

## ��ʾ
���� $100\%$ �����ݣ��� $n \le 1 \times 10^5$��

