## ��Ŀ����


There is an urban myth that Peter the Great wanted to make a rectangular channel-grid engineering masterpiece not only from Vasilyevskiy island, but also from Kotlin island (where the town of Kronstadt is located nowadays).

The following mathematical model was (allegedly) presented to the tsar. The island is considered a rectangular grid $h$ cells high and $w$ cells wide. Each cell is dry land initially but can become water.

Technologies of those days allowed engineers to dig a channel across the entire island. In that case an entire row or an entire column of cells became water. If some of these cells already were water, their status did not change.

Your task is to propose a plan of the island which has exactly $n$ connected components of dry land cells.



## �����ʽ


The only line of the input contains three integers $h , w$ , and $n$ -- grid's height, width and the desired number of connected components $(1 \le h , w \le 100$ ; $1 \le n \le 10^{9}).$



## �����ʽ


If there is no valid plan containing $n$ connected components, output a single word `Impossible`.

Otherwise output $h$ lines of length $w$ depicting the plan. Dot $(��. ')$ represents a dry land cell, hash $(��#')$ represents a water cell.



## ��Ŀ����
����һ�� $h$ �� $w$ �е�����ÿ�����Ӷ��ǡ�����ġ���

���ÿ�β������԰�ĳһ�л�ĳһ�е����и��ӱ�ɡ�ʪ��ġ���

���Ŀ����������������**ǡ��** $n$ ���ɡ�����ġ������γɵ���ͨ�顣

�������ʵ�֣��������һ�� $h$ �� $w$ �еľ���
���У��� `.` ��ʾ������ġ����ӣ� `#` ��ʾ��ʪ��ġ����ӡ�

�������һ��һ�� `Impossible` ��ʾ������ʵ��Ŀ�ꡣ

```input1
3 5 4

```

```output1
..#..
#####
..#..

```

```input2
2 1 1

```

```output2
#
.

```

```input3
5 3 10

```

```output3
Impossible

```

## ��ʾ
Time limit: 3 s, Memory limit: 512 MB. 



