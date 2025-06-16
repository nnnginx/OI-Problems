## ��Ŀ����
�����롣��������ṩ������������������ֱ�ӷ����ۣ���л��Ĺ��ס�


## ��Ŀ����
Farmer John's cows would like to host a dance party in their barn, complete with a laser light show.  Unfortunately, the only working laser they have found is located far away from the barn and too heavy to move, so they plan to re-direct the laser light to the barn using a series of mirrors.

The layout of the farm has the laser at position (0,0) pointing north (in the positive y direction), and the barn at (Bx, By); we can think of both the laser and the barn as points in the 2D plane.  There are already N cows (1 <= N <= 100,000) scattered throughout the farm holding mirrors that are aligned at angles of 45 degrees to the axes.  For example, a mirror aligned like \ will take a beam of light entering from below and reflect it to the left.  We can also think of the mirrors as being located at points in the 2D plane.

Just before pressing the big red button to activate the laser, Bessie noticed a major flaw in the plan: the laser cannot hit the barn with the mirrors in their current configuration!  As a result, she plans to run out onto the field, and hold up one more mirror (placed once again at a 45 degree angle) in order to redirect the laser onto the barn. Please count the number of locations in the field where Bessie can stand to accomplish this goal.

All coordinates are integers between -1,000,000,000 and 1,000,000,000. It is guaranteed that any mirrors to be placed will be in this range as well. The cows running the laser insist that the beam should never come back to (0,0) after leaving this location (and with the mirrors in their initial configuration, it is guaranteed that this will not happen).  No two cows occupy the same point in space, and Bessie cannot locate herself at the same position as an existing cow.

ũ����Լ����ţ���ڹȲ�����ٰ���ᣬ�ü���������ݡ������ҵ���Ψһ�ļ������Ȳ�̫Զ�����Ұ᲻��������ţ�����þ��������伤�⣬ʹ�ü����յ��Ȳ֡�


�����λ���ڣ�0,0����ָ��Ϊ��������y�������򣩣��Ȳ���λ�ã�Bx��By�����Ѿ���Nͷ��ţ���ž��ӷ�ɢ��ũ���ĸ���λ�ã�1 <= N <= 100,000����������ԭ��֮��ļн�Ϊ45�ȡ�����һ����������\�����ľ��ӿ��԰Ѵ��·������Ĺ��߷��������Ĺ��ߡ�


Bessie�����������ǰһ����ʶ���ƻ���ȱ�ݣ��������Լ�������һ�澵�ӳ�ȥ�ˣ�ǡ��ʹ�ü����յ��Ȳ֡�


�����Bessie����վ�ڵ�λ�õ�������


���귶Χ��-1,000,000,000 �� 1,000,000,000�����ݱ�֤��ʼʱ����������ᷴ��أ�0,0��λ�á�ͬһ���ϲ������ж�ͷţ��Bessie����վ������ţ��λ�á�


## �����ʽ
\* Line 1: The integers N, Bx, and By.

\* Lines 2..N + 1: Line i+1 describes the ith mirror with 3 elements: its (x,y) location, and its orientation (either '\' or '/').

��һ�У�����������N��Bx��By��


��2~N+1�У�ÿ������������ʾţ��λ�ã�һ���ַ�����/����"\"����ʾ������ô���õġ�


## �����ʽ
where Bessie can stand to redirect the laser to the barn.

Bessie���п���վ�ڵ�λ��������


```input1
4 1 2 
-2 1 \ 
2 1 / 
2 2 \ 
-2 2 / 

```

```output1
2 

```

## ��ʾ
A mirror at (0,1) or (0,2) placed in either direction would do the trick.

������Bessie����վ�ڣ�0,1�����ߣ�0,2����

��л@SystemLLH  �ṩ����


