## ��Ŀ����


The jury has a great artistic idea -- to create a rectangular panel out of a huge pile of black and white squares of the same size. The panel should have exactly $b 4-connected$ areas made of black tiles, and $w 4-connected$ areas made of white tiles.

Remember, a $4-connected$ area of some color is a maximal set of the panel tiles such that:

any two tiles of the area share the same color;

for any two tiles of the area there is a tile sequence connecting them, such that any two consecutive tiles of the sequence share a common side.

In addition to the artistic idea, the jury has already developed a program that produces design of the panel. But since this problem is about art, any new solution is extremely important for the jury.



## �����ʽ


The only line of the input file contains two integers $b$ and $w$ -- number of black and white areas $(1 \le b , w \le 1000)$ .



## �����ʽ


The first line of the output file should contain the picture sizes $r$ and $c$ -- the number of rows and columns $(1 \le r , c \le 100 000)$ . This line should be followed by $r$ lines of $c$ symbols each. Each symbol should be either $��@'$ (for black tile) or $��. '$ (for white one). There should be no more than $100 000$ tiles in the panel.



## ��Ŀ����
���������� $b,w$�����㹹���һ���ڰ׾���ʹ�þ�����ǡ�� $b$ ����ɫ��ͨ��� $w$ ����ɫ��ͨ�顣

����ĵ�һ�а����������� $r,c$����ʾ�㹹����ľ������������������������һ�� $r\times c$ �ľ��󣬱�ʾ�㹹����ĺڰ׾������� ```@``` �����ɫ��```.``` �����ɫ��

���ݷ�Χ��$1\le b,w\le 1000$

��ľ���Ӧ���㣺$1\le r,c\le 100000$ �� $r\times c\le100000$

```input1
2 3

```

```output1
6 7
@@@@@@@
@.@@@@@
@@...@@
@@@@@@@
.......
@@@@@@@

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



