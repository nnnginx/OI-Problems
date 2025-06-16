## ��Ŀ����
To show their spirit for the holidays, the cows would like to paint a picture! Their picture will be represented as an R x C (1 <= R <= 50,000; 1 <= C <= 15) grid of unit squares, each of which is either 0 or 1. The grid rows are conveniently numbered 1..R; the columns are numbered 1..C.

Being pressed for time, the cows have asked their neighbors north of the border for help. Under the very helpful supervision of Canmuu the moose, they constructed a machine to throw paint at the picture in entire buckets! Beginning with all 0's in the picture grid, the machine splashes a certain paint color (either 0 or 1) over a

rectangle in the grid. In particular, Canmuu suggested that they perform Q (1 <= Q <= 10,000) operations; operation i consists of five integers R1\_i, R2\_i, C1\_i, C2\_i, and X\_i (1 <= R1\_i <= R2\_i <= R; 1 <= C1\_i <= C2\_i <= C; 0 <= X\_i <= 1), meaning that the cows will paint each unit square with a row index between R1\_i and R2\_i, inclusive, and a column index between C1\_i and C2\_i, inclusive, with color X\_i.

However, painting a picture like this is quite prone to mistakes. So Canmuu has enlisted you to determine, after each operation, the number of unit squares in the grid which are the correct color.

MEMORY LIMIT: 64 MB

TIME LIMIT: 1.5 seconds

Ϊ�˱����յļ��飬��ţ��Ҫ��һ���޴�Ļ���

�������Էֳ�$R\times C$�����񣬴��ϵ��±�Ϊ $1$ �� $R$ �У������ұ�Ϊ $1$ �� $C$ �С���������ɫ�����֣���ɫ���� $0$ ��ʾ�����ߺ�ɫ���� $1$ ��ʾ����

����ʱ����ȣ���ţ�ǲ��ò���̱�����ھӣ����š������͸�����һ̨������һ�β���ֻ����5������ $R1_i,R2_i,C1_i,C2_i,X_i$ $(1 \le R1_i \le R2_i \le R;1 \le C1_i \le C2_i \le C;0 \le X_i \le 1)$���� $R1_i$ �е� $R2_i$ �У�$C1_i$ �е� $C2_i$ �е�һ���󳤷���Ϳ�� $X_i$ ɫ�������в�����δ���е�ʱ�򣬻����ǰ�ɫ�ġ�

��ţ��һ��Ҫ���� $Q$ �β�����

��Ϊ�����Ļ�����Ҫ��Щ���������ţ�����������㣬ÿһ�β�������һ���ж��ٸ����������ǵ�Ŀ�껭���Ӧ�ķ�����ͬɫ�ġ�

## �����ʽ
\* Line 1: Three space-separated integers: R, C, and Q

\* Lines 2..R+1: Line i+1 contains C characters, each '0' or '1', denoting the i-th row of the grid in the obvious way.

\* Lines R+2..R+Q+1: Line R+i+1 contains five space-separated integers representing a paint operation: R1\_i, R2\_i, C1\_i, C2\_i, and X\_i


## �����ʽ
\* Lines 1..Q: On line i+1, print a single integer representing the number of matching unit squares after the i-th operation.


```input1
17 15 10 
111111101111111 
111111000111111 
111110000011111 
111100000001111 
111000000000111 
111100000001111 
111000000000111 
110000000000011 
111000000000111 
110000000000011 
100000000000001 
110000000000011 
100000000000001 
000000000000000 
111111000111111 
111111000111111 
111111000111111 
5 8 2 14 1 
8 17 3 7 1 
4 5 10 15 0 
7 16 12 14 1 
2 17 13 14 0 
2 6 2 3 1 
13 14 4 8 1 
3 6 6 7 1 
1 16 10 11 0 
7 16 10 10 0 

```

```output1
113 
94 
95 
91 
87 
93 
91 
87 
93 
93 

```

## ��ʾ
The cows want to paint a picture of a holiday tree


After the first operation, the picture grid looks as follows:

000000000000000

000000000000000

000000000000000

000000000000000

011111111111110

011111111111110

011111111111110

011111111111110

000000000000000

000000000000000

000000000000000

000000000000000

000000000000000

000000000000000

000000000000000

000000000000000

000000000000000

There are 113 unit squares which match the corresponding square in the tree image; they are denoted below by an 'x' (the other bits are shown as they appear after the first paint splash):

0000000x0000000

000000xxx000000

00000xxxxx00000

0000xxxxxxx0000

0xx111111111xx0

0xxx1111111xxx0

0xx111111111xx0

0x11111111111x0

000xxxxxxxxx000

00xxxxxxxxxxx00

0xxxxxxxxxxxxx0

00xxxxxxxxxxx00

0xxxxxxxxxxxxx0

xxxxxxxxxxxxxxx

000000xxx000000

000000xxx000000

000000xxx000000


