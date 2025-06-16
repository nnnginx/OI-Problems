## ��Ŀ����
You have a treasure map that is arranged into a $N \times M$ grid. A grid square may be either sea or part of an island. In addition, the map shows the treasure and an enemy Viking ship that occupies one (sea) square. Finally, for convenience you have also drawn your own position.

Now you must set up a fixed route to get the treasure. The route must start at your position, end at the treasure, and consist of a sequence of moves. In each move, you can go only to an (horizontally or vertically) adjacent square that is not part of an island. But beware: The Viking ship might follow you, using the same kind of moves! After each of your moves according to your route, the Viking ship may move or not. Your move and the Vikings�� reaction together is called a round.

After every round, the following checks are made:

-    If you are in line with the Viking ship (you are in the same vertical or horizontal line as the Viking ship with only sea between the Viking ship and you), you are dead.
-    If you aren��t dead and at the treasure-spot, you get the treasure.

Write a program that decides whether it is possible to set up a fixed route in advance such that you can get the treasure by following this route and will not get killed by the Vikings �C no matter how the Viking ship moves.

## �����ʽ
The first line of input contains two integers $N$ and $M$, the dimensions of the map. Each of the following $N$ lines contain $M$ characters. Each character describes a square in the map, and is either ``.`` (sea), ``I`` (part of an island), ``V`` (the Viking ship), ``Y`` (your position), or ``T`` (the treasure). Each of ``V``, ``Y``, and ``T`` will occur exactly once.

## �����ʽ
The only line of the output must contain the string ``YES``, if it is possible to set up a route to get the treasure, or ``NO`` otherwise.

## ��Ŀ����
����һ�Ųر�ͼ���ر�ͼ����Ϊ $N��M$ ������ÿ�����ӿ�������Ĵ�������������½�ػ�ر��㡣��ֻ��һ����������ͼֻ��һ�����������������ֻ���ں����ƶ����ر����ں��С�

�������������ƶ���ÿһ�غϣ����ƶ�һ�Σ����������ƶ�һ�Ρ�ÿ���ƶ���������ƶ������������ĸ����ڸ����е�һ��Ҳ���Բ��ƶ����������ƶ�ͬ������Ҳ���Բ��ƶ��������ƶ���

ÿһ�غϽ�����������������ͬһ�л�ͬһ�У�**�����������֮��û��½��**����͹��ˣ�����û�ҵ�����£������λ�ڲر��㣬����õ��˱��ء�  
���ʣ��Ƿ���һ����ȫ��·����ʹ������������ô���㶼�ܻ����õ����ء�

Translated by @Planet6174

```input1
5 7
Y.....V
..I....
..IIIII
.......
...T...
```

```output1
YES
```

```input2
5 7
Y....V.
..I....
..IIIII
.......
...T...
```

```output2
NO
```

```input3
2 3
.YT
VII
```

```output3
NO
```

## ��ʾ
**Sample Explanation 1**

The route is:go down for three times,go right for three times too,go down at last.

**���ݷ�Χ**

���� $50\%$ �����ݣ�$1 \le N,M \le 200$��

�����������ݣ�$1 \le N,M \le 700$��

