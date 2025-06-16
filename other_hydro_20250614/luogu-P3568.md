## ��Ŀ����
A snake fills a ![](http://main.edu.pl/images/OI21/waz-en-tex.1.png) board completely.

Successive segments of the snake are numbered from ![](http://main.edu.pl/images/OI21/waz-en-tex.2.png) to ![](http://main.edu.pl/images/OI21/waz-en-tex.3.png).

The segments with successive numbers (i.e., 1 and 2, 2 and 3, 3 and 4...) occupy squares  that share an edge.

For example, a snake can fill a ![](http://main.edu.pl/images/OI21/waz-en-tex.4.png) board as follows:

The snake's segment numbers in some of the squares have been erased.

  Can you reconstruct the snake?

һֻ�߱�������һ��3\*n��ľ���ϣ�������ˣ����߱���Ϊ���С�Σ�С�εı����1��3n������˵�߿�����дһ��3\*9��ľ�壬������ʾ��


����ľ���ϵ��߶���ɾ�ڵ���


�����ؽ�����


## �����ʽ
In the first line of the standard input, there is a single integer ![](http://main.edu.pl/images/OI21/waz-en-tex.5.png)  (![](http://main.edu.pl/images/OI21/waz-en-tex.6.png)), the length of the board.

The three lines that follow describe the board;  the ![](http://main.edu.pl/images/OI21/waz-en-tex.7.png)-th of them contains ![](http://main.edu.pl/images/OI21/waz-en-tex.8.png) integers ![](http://main.edu.pl/images/OI21/waz-en-tex.9.png)  (![](http://main.edu.pl/images/OI21/waz-en-tex.10.png) for ![](http://main.edu.pl/images/OI21/waz-en-tex.11.png)).

If ![](http://main.edu.pl/images/OI21/waz-en-tex.12.png), then ![](http://main.edu.pl/images/OI21/waz-en-tex.13.png) is the number of the snake's segment  occupying the ![](http://main.edu.pl/images/OI21/waz-en-tex.14.png)-th square of the ![](http://main.edu.pl/images/OI21/waz-en-tex.15.png)-th row of the board.

If on the other hand ![](http://main.edu.pl/images/OI21/waz-en-tex.16.png), then the number of the snake's segment  on this square is unknown.

In tests worth 15% of the total score ![](http://main.edu.pl/images/OI21/waz-en-tex.17.png) holds,  in those worth 40% of the total score ![](http://main.edu.pl/images/OI21/waz-en-tex.18.png) holds,  and finally, in those worth 70% of the total score ![](http://main.edu.pl/images/OI21/waz-en-tex.19.png) holds.

�ڱ�׼����ĵ�һ���У���һ������n��1<=n<=1000��������ĳ��ȡ�


������������ľ����������i����n������aij��0<=aij<=3n��(1<=j<=n)��


���aij����0����ôaij�����߶εĵ�aij����


���aij=0����ô����߶ξ������ǲ�֪����


## �����ʽ
Your program is to print three lines to the standard output.

The ![](http://main.edu.pl/images/OI21/waz-en-tex.20.png)-th lines should hold ![](http://main.edu.pl/images/OI21/waz-en-tex.21.png) positive integers ![](http://main.edu.pl/images/OI21/waz-en-tex.22.png) (for ![](http://main.edu.pl/images/OI21/waz-en-tex.23.png)).

All the numbers ![](http://main.edu.pl/images/OI21/waz-en-tex.24.png) together should be a permutation of the numbers from ![](http://main.edu.pl/images/OI21/waz-en-tex.25.png) to ![](http://main.edu.pl/images/OI21/waz-en-tex.26.png).

The output numbers should be a valid reconstruction of the snake, i.e., they should  be consistent with the (positive) input numbers and satisfy aforementioned constraints.

You may assume that there is at least one valid reconstruction of the snake.

If there is more than one, your program can print any valid reconstruction.

������aijΪ0���߶β���


```input1
9
0 0 5 0 17 0 0 0 21
8 0 0 3 16 0 0 25 0
0 0 0 0 0 0 0 0 23

```

```output1
7 6 5 4 17 18 19 20 21
8 1 2 3 16 15 26 25 22
9 10 11 12 13 14 27 24 23

```

