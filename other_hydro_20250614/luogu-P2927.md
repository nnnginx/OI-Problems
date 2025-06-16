## ��Ŀ����
The cows have taken up alphabetical jigsaw puzzles. In these puzzles with R (1 <= R <= 10) rows and C (1 <= C <= 10) columns, the edges are not funny-shaped cardboard shapes but rather are letters.

Each piece has a serial number and 4 letters (or borders) that must be aligned as in a regular jigsaw puzzle. The pseudo-letter '0' (the digit 0) will represent a border (and a piece can have several borders if it is a corner piece or even the top of column in a, e.g., 4x1 puzzle).  Below is a set of six pieces (the borders are marked with lines instead of '0's) assembled in one way (of many) that completes the puzzle:

+---+  +---+  +---+

| 1 c  c 3 d  d 5 | 
+-d-+  + a +  +-e-+

+-d-+  +-a-+  +-e-+

| 2 b  b 4 b  b 6 | 
+---+  +---+  +---+

Note that each edge letter of each piece matches the border letter of the piece adjacent to it; the borders appear properly on the top, bottom, and sides.

Pieces are represented by a serial number and a clockwise list of their four edges (where edges are the letters a..z and 0). Pieces might require rotation when placed in the puzzle.

Given a set of pieces, find at least one way to assemble them into a puzzle. Test data for puzzles with larger R and C are easier to solve because they have a more varied set of edge letters.

��ţ�����水��ĸ��˳�����е�ƴͼ����.ÿ��������R(1��R��10)��C(1��C��10)�е�ƴͼ��,���Ǳ�Ե������ĸ���ձ߽����,��ɺ������ƴͼ��Χ�Ǳ߽���,�м�ı߽�����ĸ.

ÿ��ƴͼ�鶼��һ�����кź�4����ĸ�������ֱ�ʾ�߽���(˳��Ϊ��������),��������,���ֳ䵱�߽���.

ƴͼ���Ի�λ����ת,��ɺ��ƴͼ�ڱ�Ե�Ŀ��Ͽ�����Χ���Ǳ߽���,ƴͼ��ɺ�,һ��ƴͼ������һ������,���ǵı߽���ĸ������ͬ,������һϵ���Ѿ��ɹ���ɵ�ƴͼ���⹲6��.


## �����ʽ
\* Line 1: Two space-separated integers: R and C

\* Lines 2..R\*C+1: Each line contains five space-separated entities: an integer serial number and four edge identifiers


## �����ʽ
\* Lines 1..R\*C: Line R\*(i-1)+j describes the puzzle piece placed a row i, column j with an integer and five space-separated entities: the serial number of the puzzle piece and the four piece edge identifiers in the order top, right, bottom, left.


```input1
2 3 
1 c d 0 0 
2 0 d b 0 
3 c 0 d a 
4 b a b 0 
5 d 0 0 e 
6 0 0 b e 

```

```output1
1 0 c d 0 
3 0 d a c 
5 0 0 e d 
2 d b 0 0 
4 a b 0 b 
6 e 0 0 b 

```

## ��ʾ
Describes the input puzzle although with some of the pieces rotated compared to the sample solution.


As shown in the diagram in the task text. Other solutions (like reflections) are possible; a grading program will check your answer.


