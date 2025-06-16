## ��Ŀ����
��Peter Pan frames�� are a way of decorating text in which every character is framed by a diamond shaped frame, with frames of neigbhouring characters interleaving. A Peter Pan frame for one letter looks like this ('X' is the letter we are framing):
```
..#..
.#.#.
#.X.#
.#.#.
..#..
```
However, such a framing would be somewhat dull so we'll frame every third letter using a ��Wendyframe��. A Wendy frame looks like this:

```
..*..
.*.*.
*.X.*
.*.*.
..*..
```
When a Wendy frame interleaves with a Peter Pan frame, the Wendy frame (being much nicer) is put on top. For an example of the interleaving check the sample cases.

## �����ʽ
The first and only line of input will contain at most 15 capital letters of the English alphabet.

## �����ʽ
Output the word written using Peter Pan and Wendy frames on 5 lines.

## ��Ŀ����
���˵á��˿�ܡ���һ��װ�����֣�ÿһ����ĸ������һ�����ο�ܡ�һ���˵á��˿�ܿ����������� ��x����ĸ��#�ǿ�ܣ���
```
..#..
.#.#.
#.X.#
.#.#.
..#..
```
Ȼ����ֻ��һ����ܻ���Щ���ƣ���������ÿ����������ĸ��ѵ�������ĸ���µϿ�ܰ������������µϿ�ܿ�������������
```
..*..
.*.*.
*.X.*
.*.*.
..*..
```
���µϺͱ˵á��˵Ŀ���ص�ʱ���µϿ�ܸ��������档 ��������3��4��

�����ʽ�� һ�а�������15��Ӣ����ĸ�Ĵ�д��ĸ��

�����ʽ�� ���ʹ�ñ˵á��˺��µϿ��д�ɵ�5�����֡�

```input1
A
```

```output1
..#..
.#.#.
#.A.#
.#.#.
..#..
```

```input2
DOG
```

```output2
..#...#...*..
.#.#.#.#.*.*.
#.D.#.O.*.G.*
.#.#.#.#.*.*.
..#...#...*..
```

```input3
ABCD
```

```output3
..#...#...*...#..
.#.#.#.#.*.*.#.#.
#.A.#.B.*.C.*.D.#
.#.#.#.#.*.*.#.#.
..#...#...*...#..
```

