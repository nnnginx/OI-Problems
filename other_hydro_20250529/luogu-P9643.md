## ��Ŀ����
Grid City is a city on an infinite two-dimensional plane, where for all $k \in \mathbb{Z}$ ($\mathbb{Z}$ is the set of all integers) lines $x = k$ and $y = k$ are the streets of the city. People can only move along the roads to go from one position to another. That's why the city is called the Grid City!

Two friends, BaoBao and DreamGrid, live happily in the city. Today BaoBao is heading from his home positioned at $(x_A, y_A)$ ($x_A, y_A \in \mathbb{Z}$) towards the shopping mall positioned at $(x_C, y_C)$ ($x_C, y_C \in \mathbb{Z}$). However, it's too far for him to walk there, so he decides to call DreamGrid whose home is positioned at $(x_B, y_B)$ ($x_B, y_B \in \mathbb{Z}$) for help.

BaoBao and DreamGrid set out separately from their homes at the same time. Different from BaoBao who walks at a speed of $a$ units per minute, DreamGrid drives a car and moves at a speed of $b$ units per minute. When DreamGrid and BaoBao meet at the same point, DreamGrid can pick up BaoBao and they can then move at a speed of $b$ units per minute together. It takes no time to turn around or pick up BaoBao.

What's the minimum time needed for BaoBao to go from his home to the shopping mall? Note that it's NOT necessary for DreamGrid to pick up BaoBao if it will be faster for BaoBao to get to the destination.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$($ 1 \le T \le 10^5$), indicating the number of test cases. For each test case:

The first line contains two integers $a$ and $b$ ($1 \le a < b \le 10^9$), indicating the walking speed of BaoBao and the driving speed of DreamGrid.

The second line contains six integers $x_A$, $y_A$, $x_B$, $y_B$, $x_C$ and $y_C$ ($-10^9 \le x_A, y_A, x_B, y_B, x_C, y_C \le 10^9$), indicating the position of BaoBao's home, DreamGrid's home and the shopping mall. It's guaranteed that these three points are different from each other.

## �����ʽ
For each test case output one line containing one number, indicating the shortest time for BaoBao to arrive at the shopping mall. Your answer will be considered correct if its absolute or relative error does not exceed $10^{-6}$.

## ��Ŀ����
**����Ŀ������**

���ӳ���һ��λ�����޶�άƽ���ϵĳ��У����ж������� $k \in \mathbb{Z}$��$\mathbb{Z}$ �����������ļ��ϣ���ֱ�� $x = k$ �� $y = k$ �ǳ��еĽֵ�������ֻ�����ŵ�·��һ��λ���ƶ�����һ��λ�á������Ϊʲô������б���Ϊ���ӳǣ�

�������ѣ�������������ӣ����ֵ������������������챦��������λ�� $(x_A, y_A)$��$x_A, y_A \in \mathbb{Z}$���ļҳ�����ǰ��λ�� $(x_C, y_C)$��$x_C, y_C \in \mathbb{Z}$���Ĺ������ġ�Ȼ�������·������˵̫Զ�ˣ�������������ס�� $(x_B, y_B)$��$x_B, y_B \in \mathbb{Z}$���������������æ��

�������������ͬʱ�����ǵļҳ�������ͬ����ÿ���� $a$ ����λ�ٶȲ��еı�����������ӿ�������ÿ���� $b$ ����λ�ٶ��ƶ�����������Ӻͱ�����ͬһ��������ʱ��������ӿ��Խ��ϱ�����Ȼ�����ǿ���һ����ÿ���� $b$ ����λ�ٶ��ƶ���ת�����ϱ�������Ҫʱ�䡣

�ӱ����ļҵ�����������������ʱ���Ƕ��٣���ע�⣬���������ӽ��ϱ��������������Ҫ������ӽӱ�����


**�������ʽ��**

�ж����������������ĵ�һ�а���һ������ $T$��$1 \le T \le 10^5$������ʾ��������������������ÿ������������

��һ�а����������� $a$ �� $b$��$1 \le a < b \le 10^9$������ʾ�����Ĳ����ٶȺ�������ӵļ�ʻ�ٶȡ�

�ڶ��а����������� $x_A$��$y_A$��$x_B$��$y_B$��$x_C$ �� $y_C$��$-10^9 \le x_A, y_A, x_B, y_B, x_C, y_C \le 10^9$������ʾ�����ļҡ�������ӵļҺ͹������ĵ�λ�á���֤�����㻥����ͬ��

**�������ʽ��**

����ÿ���������������һ�У�����һ�����֣���ʾ�������ﹺ�����ĵ����ʱ�䡣�����Ĵ𰸵ľ���������������� $10^{-6}$���򽫱���Ϊ��ȷ��

**���������͡�**

���ڵ�һ����������������������������ӽ��� $D(1,2)$ ������Ȼ������������ű���ȥ�������ġ�

���ڵڶ�����������������������������ӽ��� $D(1.5,1)$ ������Ȼ������������ű���ȥ�������ġ�

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
3
1 2
0 2 1 0 2 2
1 3
1 1 0 1 3 1
1 2
0 0 100 100 1 1
```

```output1
1.500000000000000
1.000000000000000
2.000000000000000
```

## ��ʾ
For the first sample test case, BaoBao and DreamGrid will meet at $D(1,2)$ and then DreamGrid drives BaoBao to the shopping mall.

For the second sample test case, BaoBao and DreamGrid will meet at $D(1.5,1)$ and then DreamGrid drives BaoBao to the shopping mall.

![](https://cdn.luogu.com.cn/upload/image_hosting/wexb0vmz.png)

