## ��Ŀ����
��Ŀ����(by:���峼)��


ƽ������(0,0)��(n,m)��(n+1)\*(m+1)���㡣���ж��ٵ���������߶β��������㣬�ҳ�����[l,h]��Χ�ڡ�


## ��Ŀ����
Bessie is returning from a long trip abroad, and Farmer John wants to erect a nice 'Welcome Home' banner in her pasture for her arrival. The banner will hang between two poles on a wire whose length is in the range L1..L2 (1 <= L1 <= L2; L1 <= L2 <= 1,500).

The pasture's size is W x H (1 <= W <= 1,000; 1 <= H <= 1,000), and Farmer John has installed a post at every point with integer

coordinates. Of these (W + 1) \* (H + 1) points, Farmer John must pick just two that will hold either end of the wire from which he will hang the banner.

FJ wants no interference with his banner as it hangs and requires that no post be directly under the tight wire he stretches between the two chosen posts.

Farmer John needs your help to figure out how many possible ways he can hang the banner. He knows the number is large and that a 32-bit integer might not be sufficient to compute the answer.

Consider the example pasture below, with W = 2 and H = 1: 

\* \* \*
\* \* \*
The banner size is in the range 2..3. This pasture contains (2+1) \* (1+1) = 6 points and has (6 take 2) = (6\*5)/(2\*1) = 15 different potential pairs of points between which the banner-holding wire might stretch:

```cpp
(0,0)-(0,1)   (0,0)-(2,1)   (0,1)-(2,1)   (1,1)-(2,0) 
(0,0)-(1,0)   (0,1)-(1,0)   (1,0)-(1,1)   (1,1)-(2,1) 
(0,0)-(1,1)   (0,1)-(1,1)   (1,0)-(2,0)   (2,0)-(2,1) 
(0,0)-(2,0)   (0,1)-(2,0)   (1,0)-(2,1) 
```
Of these pairs, only four have a length in the range 2..3:
Len                       Len

(0,0)-(2,0) 2.00          (0,1)-(2,0) 2.24 

(0,0)-(2,1) 2.24          (0,1)-(2,1) 2.00 

Of these four, the pairs (0,0)-(2,0) and (0,1)-(2,1) both have a post directly on the line between the endpoints, and thus are 

unsuitable.

So, just two pairs of points out of 15 are acceptable candidates for hanging the banner wire.


## �����ʽ
\* Line 1: Four space-separated integers: W, H, L1, and L2


## �����ʽ
\* Line 1: A single integer denoting the number of possible banners


## ��Ŀ����
������Ҫ��һ�˳�;�����л�����Farmer John��Ҫ�����������ﲼ��һ������ӭ�ؼҡ��ĺ����ӭ����������������˩��һ����ΧΪL1��L2 (1 <= L1 <= L2; L1 <= L2 <= 1,500)���ߵ�����

�������ΪW �� H (1 <= W <= 1000;1 <= H <= 1000)������Farmer John��ÿ����������ĵ㶼��װ��һ�����ӡ�����(W + 1) * (H + 1)���У�Farmer John����ѡ�����������̶������������ĵ��ߵ����ˡ�

FJϣ���������Ĺ���ȥ֮�󲻻ᱻ��ס����������������֮������ϲ������������ӡ�

Farmer John��Ҫ��İ�������������ж����ֿ��ܵķ�ʽ�����Һ������֪��������ֺܴ�һ��32λ���������ܲ����Լ�����𰸡�

ʾ����W = 2, H = 1: �����С��2��3�ķ�Χ�ڡ������������(2+1)(1+1)= 6���㣬������(6ѡ2)=(65)/(2*1)= 15����ͬ��Ǳ�ڵ�ԣ�����Щ��֮����������⼸����:


(0,0)-(0,1)   (0,0)-(2,1)   (0,1)-(2,1)   (1,1)-(2,0) 
(0,0)-(1,0)   (0,1)-(1,0)   (1,0)-(1,1)   (1,1)-(2,1) 
(0,0)-(1,1)   (0,1)-(1,1)   (1,0)-(2,0)   (2,0)-(2,1) 
(0,0)-(2,0)   (0,1)-(2,0)   (1,0)-(2,1)
����Щ���У�ֻ���ĸ��ĳ�����2..3�ķ�Χ��:

(0,0)-(2,0) 2.00

(0,1)-(2,0) 2.24

(0,0)-(2,1) 2.24

(0,1)-(2,1) 2.00

�����ĸ��У�(0,0)-(2,0)��(0,1)-(2,1)�ڶ˵�֮���ֱ���϶���һ�����ӣ�����ǲ����ʵġ�

���ԣ�15�Ե���ֻ�����Ե������Ϊ���Һ���ߵĺ�ѡ�㡣

```input1
2 1 2 3 

```

```output1
2 

```

