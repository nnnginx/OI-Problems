## ��Ŀ����
Farmer John has purchased the world's most loathesome hay baler. Instead of having a drive-roller that drives maybe an idler roller that drives the power take-off for the baler, it has N rollers (2 <= N <= 1050) which drive and are driven by various rollers.

FJ has meticulously cataloged data for each roller i: X\_i,Y\_i are the center of the roller (-5000 <= X\_i <= 5000; -5000 <= Y\_i <= 5000); R\_i is the roller's radius (3 <= R\_i <= 800). The drive-roller is located at 0,0; the baler power take-off is located at X\_t,Y\_t (numbers supplied in the input).

The drive-roller turns clockwise at 10,000 revolutions per hour. Your job is to determine the speeds of all the rollers that are in the power-train: from the drive-roller through the power take-off roller. Rollers that do not transfer power to the take-off roller are to be ignored. A roller of radius Rd that is turning at S rph and driving another roller of radius Rx will cause the second roller to turn at the speed -S\*Rd/Rx (where the sign denotes whether the roller is turning clockwise or counterclockwise (anticlockwise for our British friends)).

Determine the power-train path and report the sum of the absolute values of all those rollers' speeds. All the rollers in the input set except the driver-roller are driven by some other roller; power is never transferred to a roller from more than one other roller.

Report your answer as an integer that is the truncated value after summing all the speeds.

## �����ʽ
\* Line 1: Three space-separated integers: N, X\_t, and Y\_t

\* Lines 2..N+1: Line i+1 describes roller i's properties: X\_i, Y\_i, and R\_i

## �����ʽ
\* Line 1: A single integer that is the truncated version of the sum of the absolute value of the speeds of the rollers in the power-train including the drive-roller, all the driven rollers, and the power take-off roller.

## ��Ŀ����
Farmer John ����ĸɲݴ�������ڲ��ṹ���������������ҵ��ˣ���������ͨ�Ļ���һ������ȷ���ڲ�����װ�ã����� $N$ �����ֻ������ã�ÿ�����ֶ����������Ŷ�����֡� FJ ��¼�˶���ÿ������ $i$����¼������ $3$ ����������һ����Ԫ�� $(x,y,r)$ ��ʾ��$x$ �� $y$ ��ʾ�������ĵ�λ�����꣬$r$ ��ʾ�ó��ֵİ뾶��

�������ֵ�λ��Ϊ $(0,0)$������ FJ Ҳ֪�����յĹ�������λ�� $(X_t,Y_t)$�� ��������˳ʱ��ת����ת��Ϊ $10,000$ ת/Сʱ����������ǣ�ȷ���������������г��ֵ�ת�١��������еĶ���Ϊ���������������ִ��͵��������ֵĹ������õ������г��ֵļ��ϡ�����������������ĳ��ֶ�Ӧ�������ԡ�

��һ���뾶Ϊ $R_d$��ת��Ϊ $S$ ת/ÿСʱ�ĳ��ֵĴ����£�������ӵİ뾶Ϊ $R_x$ �ĳ��ֵ�ת�ٽ�Ϊ $-S\times \frac{R_d}{R_x}$ ת/Сʱ��$S$ ǰ�ĸ��ŵ���˼�ǣ�һ�����ִ�������һ�����ֵ�ת���������ת���෴��

FJ ֻ�������������������г����ٶȵľ���ֵ֮�͸���Ȥ���������Ҳ����Ӧת���������ֵ�������г�������������������г��ֶ�������ĳ�����ִ��������Ҳ������ $2$ ����ͬ�ĳ��ִ���ͬһ�����ֵ������

### �����ʽ

��һ�У������������ֱ���� $N,X_t,Y_t$��

�� $2$ �е��� $N+1$ �У�ÿ����������������һ����Ԫ�� $(x,y,r)$��

### �����ʽ

�����һ�У�һ�����������������������������г����ٶȵľ���ֵ֮�͡�

```input1
4 32 54 
0 0 10 
0 30 20 
32 54 20 
-40 30 20 

```

```output1
20000 

```

## ��ʾ
$2 \leq N \leq 1050$��$-5000 \leq x,y \leq 5000$��$3 \leq r \leq 800$��




Four rollers: the drive-roller at 0,0 with radius 10. It drives the roller above it at 0,30 with radius 20. That roller drives both the power take-off roller at 32,54 (r=20) and a random roller (not in the power train) at -40,30 (r=20).


Roller   Radius   Speed

1 (0,0)     10     10,000 

2 (0,30)    20     -5,000 

3 (32,54)   20      5,000 

------
Sum of abs values: 20,000


