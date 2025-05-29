## ��Ŀ����
Farmer John's cows recently received a large piece of marble, which, unfortunately, has a number of imperfections.  To describe these, we can represent the piece of marble by an N by N square grid (5 <= N <= 300), where the character '\*' represents an imperfection and '.' represents a flawless section of the marble.

The cows want to carve a number "8" in this piece of marble (cows are quite fond of the number "8" since they have cloven hooves on each of their four feet, so they can effectively count up to 8 using their "toes"). However, the cows need your help to determine the optimally placed figure eight in the piece of marble.  Here are a few properties that define a valid figure eight:

\* A figure eight consists of two rectangles, a top and a bottom. \* Both the top and bottom have at least one cell in their interior. \* The bottom edge of the top rectangle is a (not necessarily proper) subset of the top edge of the bottom rectangle.

\* The figure eight can only be carved from flawless regions of the piece of marble.

The aesthetic score of a figure eight is equal to the product of the areas enclosed by its two rectangles.  The cows wish to maximize this score.

```cpp
............... 
............... 
...*******..... 
.*....*.......* 
.*......*....*. 
....*.......... 
...*...****.... 
............... 
..**.*..*..*... 
...*...**.*.... 
*..*...*....... 
............... 
.....*..*...... 
.........*..... 
............... 
```
For example, given this piece of marble 

the optimally placed eight is:

```cpp
..88888888888.. 
..8.........8.. 
..8*******..8.. 
.*8...*.....8.* 
.*8.....*...8*. 
..8.*.......8.. 
..8*...****.8.. 
.88888888888888 
.8**.*..*..*..8 
.8.*...**.*...8 
*8.*...*......8 
.8............8 
.8...*..*.....8 
.8.......*....8 
.88888888888888 
```
The top rectangle has area 6x9=54, and the bottom rectangle has area 12x6=72.  Thus, its aesthetic score is 54x72=3888.

ũ��Լ������ţ����յ���һ������ʯ�����ҵ��ǣ��������ȱ��.��Ϊ��������Щ�����ǿ�����n����������������ʾһ�����ʯ��5 < n = n = 300���������ַ���\*����ʾһ���������͡���


ĸţ����һ�����롰8������һ�����ʯ��ţ��ϲ�����֡�8������Ϊ���Ƕ����ǵ�ÿһ����Ӣ�ߣ���ż����Ч������8���á��š�����Ȼ������ţ��Ҫ��İ�������ȷ����ѷ�����ͼ�˿����ʯ��������һЩ���Զ���һ����Ч�����ְˣ�


ͼ�˰����������Σ�һ��������һ���ײ��������͵ײ�������һ����Ԫ�����ڲ����������εĵײ���Ե�ǵײ����ζ�����Ե��һ������һ�����ʵ��ģ��Ӽ�.��


ͼ��ֻ�ܿ��ڴ���ʯ����覴�����


ͼ�˵���ѧ�÷ֵ�����������������Χ������ĳ˻�.����ţϣ������޶ȵ������һ�ɼ���


## �����ʽ
\* Line 1: A single integer N, indicating the side length of the marble.

\* Lines 2..N+1: Each line describes a row of the marble, and contains N characters which are each either '\*' (an imperfection) or '.' (a flawless section).

��1�У�һ������n����ʾ����ʯ�ı߳���


��2 N + 1��ÿ��������һ�Ŵ���ʯ��������n���ַ���ÿ�����ǡ�\*����ȱ�ݣ���'.' (����)��


## �����ʽ
\* Line 1: The highest aesthetic score of any figure eight which doesn't use any imperfect squares of the marble.  If no figure eight is attainable, then output -1.


```input1
15 
............... 
............... 
...*******..... 
.*....*.......* 
.*......*....*. 
....*.......... 
...*...****.... 
............... 
..**.*..*..*... 
...*...**.*.... 
*..*...*....... 
............... 
.....*..*...... 
.........*..... 
............... 

```

```output1
3888 

```

## ��ʾ
�����ľ������6X9 = 54���͵ײ��������12x6 = 72����ˣ�������������54x72 = 3888��


����һ��n��n������������һЩλ����覴á�����Ҫ��û��覴õ�λ���е�һ��8��������


��8���ֵĶ���Ϊ�������ο򣬿������������0����һ�����ο�ĵױ�������һ�����ο�Ķ��ߵ��Ӽ���


��������ο�������Ļ���


��л @3505515693qq �ṩ����


