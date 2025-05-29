## ��Ŀ����
Imagine Bessie's surprise as she spied a leprechaun prancing through the north pasture. Being no one's fool, she charged at the leprechaun at captured him with her prehensile hooves.

'One wish, bovine one. That's all I have for cows,' he said.

'Riches,' Bessie said dreamily. 'The opportunity for riches.'

Leprechauns never grant precisely the easiest form of their captor's wishes. As the smoke cleared from the location of a loud explosion, a shimmering donut spun slowly over the verdant green fields.

'I have made you a torus,' the leprechaun cooed. 'And on that torus is an N x N matrix (1 <= N <= 200) of integers in the range

-1,000,000..1,000,000 that will determine the magnitude of your riches. You must find the sequence of contiguous integers all in one row, one column, or on one diagonal that yields the largest sum from among all the possible sequences on the torus.'

Bessie pondered for a moment and realized that the torus was a device for 'wrapping' the columns, rows, and diagonals of a matrix so that one could choose contiguous elements that 'wrapped around' the side or top edge.

Bessie will share the matrix with you.  Determine the value of the largest possible sum (which requires choosing at least one matrix element).

By way of example, consider the 4 x 4 matrix on the left below that has all the elements from one exemplary 'wrapped' diagonal marked:

![](https://cdn.luogu.com.cn/upload/image_hosting/03z54guy.png)

The marked diagonal of the right-hand matrix includes two nines (the highest available number) and a six for a total of 24. This is the best possible sum for this matrix and includes only three of the four possible elements on its diagonal.

�����������翴��һֻ��������������ʱ�Ƕ�ô�ľ��ȣ�������ɵ�ϣ��������˹�ȥ������������ţ��ץס����ֻ������

���������һ��Ը����ɵ�������������˵��

���Ƹ��������������ΰ�������ش����  ����Ҫ��òƸ��Ļ��ᣮ��

��������û����������ô�򵥵�Ը�������ڵط�����һ���N��N(1��N��200)�ķ���ÿ��������д��\_1,000,000��1,000,000֮������֣���˵��  ���ڷ����ϳ�һ���������ߣ��������еķ����еķ���б�Խǵķ���һ��ֻ����һ��������ȹ������ֵĺ;�����ĲƸ�����

������������æ���ҵ�һ�С�һ�л�һ���Խ�������һ�����������֣����ǵĺ������������������������ԣ�����һ�������ߣ��ߵ��˱߼ʣ���һ�����ȥ���ԡ��ơ�������ĶԱ߳��֣�һ�����˵ĸ��������ڵģ�һ�����˵ĸ���Ҳ�����ڵģ������������еķֱ����˵ĸ���Ҳ�����ڵģ�б�ԽǷ��򣩣�

������ͼ��ߵķ������б�ǹ������ֶ���һ���Խ����ϣ�

  
 
������������ܲȳ��������ĺ���24���ȹ�����������ͼ�б�ǳ�����


## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 contains N space-separated integers that compose row i of the matrix


## �����ʽ
\* Line 1: A single integer that is the largest possible sum computable using the rules above


```input1
4 
8 6 6 1 
-3 4 0 5 
4 2 1 9 
1 -9 9 -2 

```

```output1
24 

```

