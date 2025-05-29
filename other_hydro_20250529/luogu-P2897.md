## ��Ŀ����
USACO 2008 January Gold

## ��Ŀ����
The oppressively hot summer days have raised the cows' clamoring to its highest level. Farmer John has finally decided to build an artificial lake. For his engineering studies, he is modeling the lake as a two-dimensional landscape consisting of a contiguous sequence of N soon-to-be-submerged levels (1 �� N �� 100,000) conveniently numbered 1..N from left to right.


Each level i is described by two integers, its width Wi (1 �� Wi �� 1,000) and height (like a relative elevation) Hi (1 �� Hi �� 1,000,000). The heights of FJ's levels are unique. An infinitely tall barrier encloses the lake's model on the left and right. One example lake profile is shown below.

          
```cpp
         *             *  :
         *             *  :
         *             *  8
         *    ***      *  7
         *    ***      *  6
         *    ***      *  5
         *    **********  4 <- height
         *    **********  3
         ***************  2
         ***************  1
Level    |  1 |2|  3   |
```
In FJ's model, he starts filling his lake at sunrise by flowing water into the bottom of the lowest elevation at a rate of 1 square unit of water per minute. The water falls directly downward until it hits something, and then it flows and spreads as room-temperature water always does. As in all good models, assume that falling and flowing happen instantly. Determine the time at which each elevation's becomes submerged by a single unit of water.


```cpp
WATER              WATER OVERFLOWS                     
       |                       |                           
     * |          *      *     |      *      *            *
     * V          *      *     V      *      *            *
     *            *      *    ....    *      *~~~~~~~~~~~~*
     *    **      *      *~~~~** :    *      *~~~~**~~~~~~*
     *    **      *      *~~~~** :    *      *~~~~**~~~~~~*
     *    **      *      *~~~~**~~~~~~*      *~~~~**~~~~~~*
     *    *********      *~~~~*********      *~~~~*********
     *~~~~*********      *~~~~*********      *~~~~*********
     **************      **************      **************
     **************      **************      **************
     After 4 mins        After 26 mins       After 50 mins

     Lvl 1 submerged     Lvl 3 submerged     Lvl 2 submerged
```
Warning: The answer will not always fit in 32 bits.

���������˴��������Ŀ��Ƚ���ţ�ǵķ��������Ƶ�����ߵ㡣���գ�FJ������һ���˹�������ţ����֮�á�Ϊ��ʹ��������������ʵ��FJ���������ĺ���潨��N(1 <= N <= 100,000)��������ƽ̨�ߵʹ�������״�����е�ƽ̨�����Ұ�1..N���α�š���Ȼ�����ں���ע��ˮ����Щƽ̨��������û��    ƽ̨i�����ͼ�������Ŀ��W\_i(1 <= W\_i <= 1,000)�͸߶ȣ���������Ϊ��ƽ̨����FJ�ڵĵػ��ĸ߶ȣ�H\_i(1 <= H\_i <= 1,000,000)�������ġ�����ƽ̨�ĸ߶ȶ��Ƕ�һ�޶��ġ����ı�Ե������Ϊ���޸ߵ�ƽ̨�����������һ��FJ�����ͼ��


��FJ�����룬�ڿ��ںú�������1��λ/���ӵ��ٶ�����͵��Ǹ�ƽ̨��עˮ��ˮ���뿪ˮ�ܺ��������䣬ֱ��ײ��ƽ̨�����Ǹ���Щʱ��ע���ˮ��Ȼ�������г����µ�ˮһ��������Ѹ�ٵ���������ɢ����������������Ϊ��Щ������˲����ɵġ�FJ��֪��������ÿһ��ƽ̨�����Ķ����Ǵ��ĸ�ʱ�̿�ʼ����ˮ��ľ�������Ϊ1��λ���ȡ�


## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 describes level i with two space-separated integers: Wi and Hi


## �����ʽ

Lines 1..N: Line i contains a single integer that is the number of minutes that since sunrise when level #i is covered by water of height 1.

```input1
3
4 2
2 7
6 4
```

```output1
4
50
26
```

