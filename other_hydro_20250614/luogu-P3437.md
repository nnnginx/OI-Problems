## ��Ŀ����
The authors of the game "Tetris" have decided to make a new, three-dimensional version, in which cuboids would fall down on a rectangular platform. The blocks fall down separately in a certain order, just like in the two-dimensional game. A block falls down until it reaches an obstacle: the platform or another block, that has already stopped - then it stops and remains in this exact position till the game is over.

However, the authors wanted to change the spirit of the game, turning it from a simple arcade-game into a play far more puzzling. Knowing the order of the falling blocks and their flight path the player's task is to tell the height of the highest point of the arrangement after all blocks have fallen down (and stopped). All the blocks are falling down vertically and do not rotate while falling. For convenience we'll introduce a cartesian coordinate system on the platform, with the center in one of the platform's corners and the axes parallel to the platform's edges.

Write a programme that automates verification of the player's answer.

TaskWrite a programme that:

reads the descriptions of subsequent falling blocks from the standard input,determines the height of the highest point of the arrangement of blocks after all have fallen down and stopped,writes the result to the standard output.



## �����ʽ
In the first line of the input there are three integers $D$, $S$ and $N$ ($1\le N\le 20\ 000$, $1\le D,S\le 1\ 000$), separated by single spaces and denoting respectively: the length and the depth of the platform and the number of blocks that are going to fall down on it. In the following $N$ lines the descriptions of subsequent blocks are given, one in each line.

Each description of a block consists of five integers: $d$,$s$,$w$,$x$ and $y$ ($1\le d$, $0\le x$, $d+x\le D$, $1\le s$, $0\le y$, $s+y\le S$, $1\le w\le 100\ 000$), representing a block of length $d$ depth $s$ and height $w$. This very block will be be falling down on the platform with its $d\times s$ face as the bottom, where the length and depth of the block are parallel to those of the platform. The coordinates of the vertices of the projection of the block on the platform are: $(x,y)$, $(x+d,y)$, $(x,y+s)$ and $(x+d,y+s)$.


## �����ʽ
The first and only line of the standard output should contain exactly one integer, the height of the highest point of the arrangement of blocks after all have fallen down and stopped.


## ��Ŀ����
### ��Ŀ����

��������˷�����һ����ά��Ķ���˹���顣�Ͷ�ά�汾���ƣ�һЩ�����尴��һ����˳����䣬ֱ��������ķ�����ǵ���Ż�ֹͣ���䡣������ֹͣ������һֱ���ֵ���ʱ��λ�ã�ֱ����Ϸ������

������Ѿ���������°汾�Ķ���˹����Ϊ��������һ���⡣����ÿ��������ĵ���˳��������Ĺ켣�������з�����ɵ���������߷���ĸ߶ȡ��������Ϸ�У��������ֱ���䣬�ҷ��鲻����ת��ת��Ϊ�˷������������ǻὨ��һ���ռ�ֱ������ϵ��������ϵ��ԭ��Ϊ�����һ�ǣ�����������������Եƽ�С�

�����ֵ�������������ˡ�

### �����ʽ

��һ���������� $D,S,N$���ֱ�Ϊ����ĳ��ȣ���ȣ��ͽ�Ҫ�����������������

������ $N$ �У�ÿ��������� $d_i,s_i,w_i,x_i,y_i$������һ������������塣���� $d_i,s_i,w_i$ �ֱ����������ĳ������ߡ�������ĵ��棨���� $\times$ �����һ�棩�����Ե��档����������ĸ����ڵ����ͶӰ����ֱ�Ϊ $(x_i,y_i)$��$(x_i+d_i,y_i)$��$(x_i,y_i+s_i)$��$(x_i+d_i,y_i+s_i)$��

### �����ʽ

���һ������������������������߷���ĸ߶ȡ�

### ���ݷ�Χ

$1 \leq N \leq 20\,000$��$1 \leq D,S \leq 1\,000$��$d_i,s_i \geq 1$��$1 \leq w_i \leq 100\,000$��$0 \leq x_i,d_i+x_i \leq D$��$0 \leq y_i,s_i+y_i \leq S$��

```input1
7 5 4
4 3 2 0 0
3 3 1 3 0
7 1 2 0 3
2 3 3 2 2
```

```output1
6
```

