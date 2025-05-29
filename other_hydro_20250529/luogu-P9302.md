## ��Ŀ����
Bocchi the Builder just finished constructing her latest project: a laneway consisting of two rows of white equilateral triangular tiles. However, at the last moment, disaster struck! She accidentally spilled black paint on some of the tiles. Now, some of the tiles are wet and the other tiles are dry. Bocchi must place warning tape around the perimeters of all wet areas. Can you help her determine how many metres of tape she needs?

The first triangular tile will point upwards. Each pair of adjacent tiles (that is, tiles that share a common side) will point in opposite directions. Each tile has a side length of $1$ metre.

## �����ʽ
The first line of input will consist of one positive integer $C$, representing the number of columns.

The next two lines will each consist of $C$ integers separated by spaces. Each integer represents
the colour of a tile along the laneway, with `1` indicating that the tile is black (wet) and `0` indicating that the tile is white (dry).

The following table shows how the available 15 marks are distributed:

| Marks | Description | Bound |
| :----------: | :---------- | :----------: |
| 3 | The laneway is not very long, black tiles are never adjacent and the second row is fully white. | $C \le 2 \times 10^3$ |
| 3 | The laneway is not very long, black tiles may be adjacent and the second row is fully white. | $C \le 2 \times 10^3$ |
| 5 | The laneway is not very long, black tiles may be adjacent and may appear in the second row. | $C \le 2 \times 10^3$ |
| 4 | The laneway may be very long, black tiles may be adjacent and may appear in the second row. | $C \le 2 \times 10^5$ |


## �����ʽ
Output a single integer representing the length of tape Bocchi needs,in metres.

## ��Ŀ����
���ʦ Bocchi �ո����һ�����̣�һ����������������ɵ������ÿһ���ֶ���һ�ű߳�Ϊ $1$ �׵������ι��ɡ���������̻���һ��С覴ã���һ���������α�Ϳ���˺�ɫ�����ǵ����ỹû�ɣ�������ʱ����ʹ�á�Bocchi ���þ����߽��ⲿ��������Χס������������Ҫ���׳��ľ����߲���Χ�ϡ�

һ��ͼ�������¾��� $C$ �������ι��ɡ�

����Ҫʵ��һ������

����һ������ $C$��$1 \leq C \leq 2 \times 10^5$�������������У�ÿ�� $C$ �����֣�`1` ��ʾ��ɫ�����Σ�`0` ��ʾ��ɫ�����Σ��������Χ�Ϻ�ɫ��������Ҫ������դ����

```input1
5
1 0 1 0 1
0 0 0 0 0
```

```output1
9
```

```input2
7
0 0 1 1 0 1 0
0 0 1 0 1 0 0
```

```output2
11
```

## ��ʾ
**��������������**��

- Subtask $1$��$3$ points����$C \leq 2 \times 10^3$����ɫ�����β����ڣ��ڶ���ȫ��Ϊ��ɫ�����Ρ�
- Subtask $2$��$3$ points����$C \leq 2 \times 10^3$����ɫ�����ο������ڣ��ڶ���ȫ��Ϊ��ɫ�����Ρ�
- Subtask $3$��$5$ points����$C \leq 2 \times 10^3$����ɫ�����ο������ڣ��ڶ��п����к�ɫ�����Ρ�
- Subtask $4$��$4$ points����$C \leq 2 \times 10^5$����ɫ�����ο������ڣ��ڶ��п����к�ɫ�����Ρ�

���� $1$ ͼ�⣺

![](https://cdn.luogu.com.cn/upload/image_hosting/5tfc7u5b.png)

���� $2$ ͼ�⣺

![](https://cdn.luogu.com.cn/upload/image_hosting/4e22mx61.png)

