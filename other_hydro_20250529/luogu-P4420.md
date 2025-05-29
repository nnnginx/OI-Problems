## ��Ŀ����
Ivica is a passionate computer scientist. He recently started working on his first computer game: a clone of the popular Tetris. Although he��s far from being finished, his program supports placing five different Tetris figures shown in the image below in a matrix. Before placing it in the Tetris matrix, the figure can be rotated by 90 degrees an arbitrary number of times and coloured. Additionally, the current version of the game doesn��t support placing the figure if that would mean it goes out of the matrix boundaries or overlaps with another existing figure in the matrix.

![](https://cdn.luogu.com.cn/upload/pic/17376.png)

While Ivica was in school, his sister Marica started the game and randomly rotated, coloured and placed the figures in a way that the adjacent figures are coloured differently. Two figures are adjacent if they share a common side or touch in the tip.

When Ivica came back to his computer, he found the game running with the figures his sister placed. He wants to know how many of which figures there are in the Tetris matrix and he is asking you to help him solve this problem while he��s busy with improving the game.


## �����ʽ
The first line of input contains positive integers N and M (1 �� N, M �� 10) that represent the number of rows and columns of the Tetris matrix.

Each of the following N lines contains M characters that represent the matrix. Each character can be ��.�� (dot) that represents a blank space or a lowercase letter of the English alphabet that represents a part of the figure. Different letters represent different colours, and the parts
of the same figure are coloured the same.


## �����ʽ
You must output exactly five rows. The $i^{th}$ line must contain the number of appearances of
the $i^{th}$ figure in the game of Tetris.


## ��Ŀ����
## ��Ŀ����

Ivica��һλ���鰺��ļ������ѧ�ҡ��������ʼ�о����ĵ�һ��������Ϸ�������ڵ��µĶ���˹����Ŀ�¡����������Զδ��ɣ��������о��ƻ�ȴ֧�ֽ���ͼ����ʾ�����ֲ�ͬ�Ķ���˹����ͼ�η���һ�������С��ڽ����������˹�������֮ǰ��ͼ�ο�����ת90�������������ɫ�����⣬��ǰ�汾����Ϸ��֧�ַ��ö���˹����ͼ�Σ��������ζ��������������߽��������е���һ������ͼ���ص���

![](https://cdn.luogu.org/upload/pic/17376.png)

��Ivica��ѧУʱ����������Marica��ʼ��Ϸ�������ת����ɫ�����ö���˹����ͼ�Σ�ʹ���ڵ���һЩ����˹������ɫ��ͬ����������ڹ���һ����ͬ�Ĳ���������ഥ��������ͼ�����ڡ���PS��������ע����Ȼ��һ������ǣ����㣩

��Ivica�ص����ĵ��Ժ���������Ϸ���������������÷��õĶ���˹����ͼ�Ρ�����֪������˹����������ж������֣���Ҫ��������æ�ڸĽ���Ϸʱ���������������⡣

## ���������ʽ

### �����ʽ��

��һ���������������N��M��1��N��M��10������ʾ����˹��������������������

����N���е�ÿһ�а�����ʾ�����M���ַ���ÿ����ɫ��������'.' ���㣩��ʾ�ո��Ӣ����ĸ��Сд��ĸ������ͼ��һ���֡���ͬ����ĸ����ͬ����ɫ��ͬһͼ�Ĳ�����ɫ��ͬ��

### �����ʽ��
�����������С��� $i^{th}$ 
 ����Ҫ����$i^{th}$ 
 ͼ�з������Ϸ�ĳ��ִ�����
 

## ˵��

20���Ĳ��������У�ֻ��һ�����֡�

�ڲ��԰����У��ܼ�ֵ��������20����Ҳ����40%����ֻ������������֡�

�ڲ��԰����У��ܼ�ֵ��������20������Ȼ��Ҳ����60%���������������֡�

�ڲ��԰����У��ܼ�ֵ��������20���������ž���80%���������ǰ�ĸ�����

![](https://cdn.luogu.org/upload/pic/17377.png)  
���빱����UID��118559

```input1
4 5
aaaa.
.bb..
.bbxx
...xx

```

```output1
2
1
0
0
0

```

```input2
4 5
.aab.
aabb.
.cbaa
cccaa

```

```output2
1
0
1
1
1

```

```input3
5 7
.c.....
ccdddd.
caabbcc
aabbacc
...aaa.

```

```output3
1
1
2
1
1
```

## ��ʾ
In test cases worth 20% of total points, only the first figure will appear.

In test cases worth an additional 20% of total points, only the first two figures will appear.

In test cases worth an additional 20% of total points, only the first three figures will appear.

In test cases worth an additional 20% of total points, only the first four figures will appear.

![](https://cdn.luogu.com.cn/upload/pic/17377.png)

