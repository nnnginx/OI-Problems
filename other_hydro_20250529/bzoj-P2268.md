## ��Ŀ����

Jonly is writing his first computer game��For the opening scene he wants to have the main character��Wormly��cross Bridgely��the bridge��Wormly is a worm made of $b$ equal circular bubbles and $L$ legs��At all times each leg has to be under one of the bubbles��and under each bubble there can be at most one leg��Bridgely was supposed to be composed of $n$ planks with the width of each plank equal to the diameter of each of Wormly's bubbles��However��some of the planks are missing��

At every moment��Wormly can do exactly one of the following��

* Move one of its legs forward over any number of��possibly missing��planks��After the move��the leg should be on a plank and underneath one of Wormly's bubbles��A leg isn't allowed to overtake other legs��

* Move all of its bubbles forward one plank while its legs remain on the same planks��After the move each leg must still be under one of Wormly's bubbles��

![](./1818/file/pic1.png)

Wormly ��һ�����ӣ����������� $b$ ����� $L$ ���ȡ��κ�ʱ��������������ĳ������·�������ÿ�����·�����һ���ȡ�

Wormly ��Ҫ���š�������ɱ����� $n$ �������ɣ����еİ��Ӳ����ˡ�

ÿ��ʱ���Wormly ��������Щ�£�

* ��ǰ�ƶ�һ���ŵ�һ����ӣ�Ҫ����Խ��ǰ����ȣ�ͼ�� `c` ��������������ʧ�İ����ϣ�ͼ�� `a` ����

* �����е�����ǰ�ƶ�һ���Ȳ���������֮��ÿ���ȱ��뻹��ĳ�����¡�

һ��ʼ��������� $b$ ������ϣ���������� $L$ ������ϣ����������ҵ� $b$ ������ϣ��������ҵ� $L$ ������ϡ������������Ҫ����ʱ�䣿

## �����ʽ

**�����ж�������**

On the first line a positive integer��the number of test cases��at most $100$��After that per test case��

One line with three integers $L,b,n$ ��the number of legs��the number of bubbles and the length of the bridge respectively��

One line with a string consisting of $n$ characters��either `0` or `1`��describing Bridgely��A one indicates a plank and a zero indicates a missing plank��

$T$����������������

$L,b$ and $n$ ��$n$ λ $01$ ����`1` �����а��ӡ�

## �����ʽ

Per test case��

One line with an integer��the minimum number of steps it takes Wormly to cross Bridgely��If it is impossible to get across while satisfying the constraints��the line must contain `IMPOSSIBLE` instead��

Figure 1��In this example��the only possible move for the last leg is to position b����The plank at position a is missing��so the leg cannot move there��To get to position c��the last leg would have to overtake the first leg����Also��in this example��moving all the bubbles forward is not allowed because Wormly's last leg would end up without a bubble over it��

Now Jonly is wondering how long the animation takes until Wormly reaches the end of Bridgely��Initially Wormly's bubbles are directly above the leftmost $b$ planks of the bridge and its legs are on the leftmost $L$ planks��At the end of the animation Wormly's bubbles have to be directly above the rightmost $b$ planks and its legs have to be on the rightmost $L$ planks��

The left- and right- most $L$ planks of Bridgely are not missing��

**IMPOSSIBLE��������С��ͨ��ʱ�䡣**

```input1
3
1 2 2
11
2 3 5
11011
1 3 5
11011
```

```output1
1
IMPOSSIBLE
5
```

## �������� 1

**�ƶ���** �� **�ƶ���** �� **�ƶ���** �� **�ƶ���** �� **�ƶ���** $5$ **��**��

## ���ݹ�ģ��Լ��

$100\%$ ���������㣺$T \le 100$��$1 \le L \le b \le n \le 1 \times 10^6$��