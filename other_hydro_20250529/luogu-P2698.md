## ��Ŀ����
Farmer John has been having trouble making his plants grow, and needs your help to water them properly.  You are given the locations of N raindrops (1 <= N <= 100,000) in the 2D plane, where y represents vertical height of the drop, and x represents its location over a 1D number line:

 ![](https://cdn.luogu.com.cn/upload/pic/9174.png) 

Each drop falls downward (towards the x axis) at a rate of 1 unit per second.  You would like to place Farmer John's flowerpot of width W somewhere along the x axis so that the difference in time between the first raindrop to hit the flowerpot and the last raindrop to hit the flowerpot is at least some amount D (so that the flowers in the pot receive plenty of water).  A drop of water that lands just on the edge of the flowerpot counts as hitting the flowerpot. 

Given the value of D and the locations of the N raindrops, please compute the minimum possible value of W.

�ϰ���Ҫ���æ���������� $N$ ��ˮ�����꣬$y$ ��ʾˮ�εĸ߶ȣ�$x$ ��ʾ�����䵽 $x$ ���λ�á�

ÿ��ˮ��ÿ�� $1$ ����λ���ȵ��ٶ����䡣����Ҫ�ѻ������ $x$ ���ϵ�ĳ��λ�ã�ʹ�ôӱ�������ŵĵ� $1$ ��ˮ��ʼ������������ŵ���� $1$ ��ˮ������֮���ʱ�������Ϊ $D$��

������Ϊ��ֻҪˮ���䵽 $x$ ���ϣ��뻨��ı��ض��룬����Ϊ����ס������ $N$ ��ˮ������� $D$ �Ĵ�С���������С�Ļ���Ŀ�� $W$��

## �����ʽ
��һ�� $2$ ������ $N$ �� $D$��

������ $N$ ��ÿ�� $2$ ����������ʾˮ�ε����� $(x,y)$��

## �����ʽ
��һ�� $1$ ����������ʾ��С�Ļ���Ŀ�ȡ�����޷�������㹻��Ļ��裬ʹ���� $D$ ��λ��ʱ���ס����Ҫ���ˮ�Σ������ $-1$��

```input1
4 5
6 3
2 4
4 10
12 15
```

```output1
2
```

## ��ʾ
�� $4$ ��ˮ��$(6,3)$ ��$(2,4)$ ��$(4,10)$ ��$(12,15)$ ��ˮ�α��������� $5$ ��ʱ�����뻨�衣����Ŀ��Ϊ $2$ �Ǳ������㹻�ġ��ѻ������ $x=4\dots6$ ��λ�ã������Խӵ� $1$ �� $3$ ˮ��, ֮���ʱ���Ϊ $10-3=7$ ����������

**�����ݷ�Χ��**

$40\%$ �����ݣ�$1 \le N \le 1000$ ��$1 \le D \le 2000$ ��

$100\%$ �����ݣ�$1 \le N \le 10 ^ 5$ ��$1 \le D \le 10 ^ 6$ ��$0\le x,y\le10^6$ ��

