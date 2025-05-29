## ��Ŀ����
Cars! Where do they come from? Where do they go? Nobody knows. They appear where roads have been built, as if out of nowhere. Some say that no two cars are alike. Some say that if you look closely, you can see the pale ghosts of miserable humans inside them, trapped forever��particularly in
the morning and late afternoon. What scientific eye could frame their fearful symmetry?

Well, yours, hopefully. As part of your government's Urban Traffic Control department, you are trying to write a paper on local traffic congestion. It is too dangerous to observe cars in the wild, of course, but you have been given some data on the traffic lights along your town's Main Street, and you would like to do some theoretical calculations about how well-synchronized they are.

Main Street is set out on a line, with traffic lights placed at various points along it. Each traffic light cycles between red and green with a fixed period, being red for $r$ seconds, then green for $g$ seconds, then red for $r$ seconds, and so on. The values of $r$ and $g$ may be different for different traffic lights. At time $0$, all the lights have just turned red.

Assume that an "ideal" car mystically appears at the west end of Main Street at a uniformly random real-valued time in the interval $[0, 2019!]$ (where $k!$ is the product of the first $k$ positive integers), driving eastwards at a slow crawl of $1$ meter/second until it hits a red light. What is the probability that it will make it through all the lights without being forced to stop? If it does hit a red light, which one is it likely to hit first?

Write a program to answer these questions.

## �����ʽ
The first line of input contains an integer $n$ ($1 \leq n \leq 500$), the number of traffic lights. Each of the following $n$ lines contains three integers $x$, $r$, and $g$ describing a traffic light, where $x$ ($1 \leq x \leq 10^5$) is the position of the light along Main Street in meters, and $r$ and $g$ ($0 \leq r, g$ and $1 \leq r + g \leq 100$) are the durations in seconds of the red and green portions of the light's period (so the light is red from time $0$ to $r$, from time $r + g$ to $2r + g$, and so on).

The west end of Main Street is at position $0$, and the lights are listed in order of strictly increasing position.

## �����ʽ
For each of the $n$ lights, output a line containing the probability that this light will be the first red light an "ideal" car hits. Then output a line containing the probability that an "ideal" car makes it all the way without stopping. Your answers should have an absolute error of at most $10^-6$.

## ��Ŀ����
### ��Ŀ����

Main ��������һ���������ֱ���ϣ�����������λ�û���ĺ��̵ơ�ÿ�����̵���ĳ���̶������ں���֮��ѭ����������أ������ȳ��� $r$ ��ĺ�ƣ��ٳ��� $g$ ����̵ƣ��ٳ��� $r$ ��ĺ��...������������ڲ�ͬ�ĺ��̵ƣ�$r$ �� $g$ ��ֵ���ܲ�ͬ����ʱ�� $0$�����еĺ��̵ƶ�ǡ�øձ�Ϊ��ơ�

�����ʱ��һ�������롱������ǰ $2019!$ ���е�һ�����ʵ��ʱ�����صس������� Main �ֵ������ˣ����� $1~ \rm m/s$ ������ʻ��ֱ��������һ�����ʱͣ�£���ô���ж��ĸ���ͨ�����к��̵ƣ������ͣ�����ˣ���ô����ÿ�����̵ƴ�ͣ�µĸ����ж��

### �����ʽ

��һ��һ������ $n$��$1\le n\le 500$�� ��ʾ���̵Ƶ�������

������ÿ���������� $x,r,g$��$1\le x \le 10^5$��$0\le r,g$ �� $1\le r+g\le 100$���� ����һ��λ���ڴ������� $x$ �״��ģ���Ƴ���ʱ��Ϊ $r$���̵Ƴ���ʱ��Ϊ $g$ �ĺ��̵ơ�

�����༴ $x=0$ ������֤ $x$ �ϸ������

### �����ʽ

ǰ $n$ �е� $i$ ��ÿ�����һ��ʵ����ʾ�ڵ� $i$ �����̵�ͣ�µĸ��ʡ�

�� $n + 1$ �����һ��ʵ����ʾͨ�����к��̵Ƶĸ��ʡ�

����Ҫ��֤���������� $10^{-6}$.

```input1
4
1 2 3
6 2 3
10 2 3
16 3 4
```

```output1
0.4
0
0.2
0.171428571429
0.228571428571
```

```input2
6
4 1 5
9 8 7
13 3 5
21 5 7
30 9 1
2019 20 0
```

```output2
0.166666666667
0.466666666667
0.150000000000
0.108333333333
0.091666666667
0.016666666667
0.000000000000
```

## ��ʾ
Source: ICPC 2019 World Finals.

