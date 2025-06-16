## ��Ŀ����
Bessie has wandered off the farm into the adjoining farmer's land. He raises delicious papaya fruit, which is a delicacy for cows. The papaya jungle is partitioned into a grid of squares with R rows and C columns (1 <= R <= 40, 1 <= C <= 40), as is popular in Wisconsin. Bessie can travel from a given square to any existing adjacent square whose route is parallel to the X or Y axis.  So in the

following diagram, if Bessie is at the square labeled 'B', she can travel to any of the squares labeled 'T':

.T.
TBT
.T.
Bessie always starts out by munching the papayas in square

(row=1,col=1).  After she's done with one square, Bessie always uses her trusty binoculars to count the low-hanging fruit in each of the adjacent squares. She then always moves to the square with the most visible uneaten fruit (a square that happily is always unique).

Sooner or later, following this rule, Bessie always ends up in square (R,C) and eats the fruit there.

Given the dimensions of the papaya jungle and the amount of fruit F\_ij in each square (1 <= F\_ij <= 100), determine the total number of fruit Bessie consumes for a given papaya jungle.

POINTS: 80

Bessie��С���ε���Farmer John����أ����߽������ڵ�ũ��ĵ��������һ��ľ�ϣ�ľ�϶���ţ��˵���ǲ��ɶ�õ���ζ�����ľ������һ�����˹�����ݵ����һ�����ָ��һ��R��C�е�����(1 <= R <= 40, 1 <= C <= 40)��Bessie���Դ�һ��������һ����X���Y��ƽ�е�ֱ���ߵ��ڽӵ���һ����Bessie����һ��ʼ���Լ���ľ���ֵ�(1,1)��Ҳ���ǵ�һ�е�һ�������Ƶؾ׽���ľ�ϡ�

Bessie����������������˫Ͳ��Զ��ȥ��ÿһ���ڽӵĸ�����ŵ�ľ�ϵ���Ŀ��Ȼ�������ε����Ǹ������û�б��Ե���ľ�ϵ��ڽӵĸ��ӣ���֤�����ĸ���ֻ��һ������

���������ƶ�����������Bessie���ǻ���(R,C)ֹͣȻ��Ե������ľ�ϡ�

�������ľ���ֵĴ�С��ÿ�����ľ����F\_ij(1 <= F\_ij <= 100), Ҫ��Bessieһ�����˶��ٸ�ľ�ϡ�


## �����ʽ
\* Line 1: Two space-separated integers: R and C

\* Lines 2..R+1: Line i+1 describes row i of the jungle with C

space-separated integers that tell how many fruit are in each square: F\_i1, F\_i2, ..., F\_iC


## �����ʽ
\* Line 1: A single integer that is the total number of papayas that Bessie eats by the time she finishes off the papayas at the barn in the lower right corner at coordinate (R,C).


```input1
3 4 
3 3 4 5 
4 5 3 2 
1 7 4 2 

```

```output1
39 

```

## ��ʾ
Three rows; four columns. Bessie starts in upper left corner at the '3'.


Bessie eats the papayas in the order given by the letters next to the numbers below:

(1,1) ---> (1,C) 

(1,1) 3a  3   4g  5h  (1,C) 

|   4b  5c  3f  2i    |

(R,1) 1   7d  4e  2j  (R,C) 

(R,1) ---> (R,C) 

She declines to eat 4 of the papayas but consumes 39 (visiting all but two squares of the grid). 



