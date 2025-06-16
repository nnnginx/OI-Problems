## ��Ŀ����


There are one hundred noble families in the country of Metagonia, and each year some of these families receive several ritual cubes from the Seer of the One. The One has several rules about cube distribution: if a family receives at least one cube, every prime divisor of the number of cubes received should be either $2$ or $3$ , moreover if one family receives a $> 0$ cubes and another family in the same year receives $b > 0$ cubes then a should not be divisible by $b$ and vice versa.

You are the Seer of the One. You know in advance how many cubes would be available for distribution for the next $t$ years. You want to find any valid distribution of cubes for each of these years. Each year you have to distribute all cubes available for that year.



## �����ʽ


The first line of input file contains a single integer $t$ -- the number of years to come $(1 \le t \le 1000)$ . Each of the following $t$ lines contains a single integer $n_{i}$ -- the number of cubes to distribute in i-th year $(1 \le n_{i} \le 10^{18}).$



## �����ʽ


For each year $i$ output two lines. The first line should contain $m_{i}$ -- the number of families that would receive at least one cube in i-th year $(1 \le m_{i} \le 100)$ . The second line should contain $m_{i}$ integers -- the number of cubes received by each family. The sum of these numbers should be equal to $n_{i}.$



## ��Ŀ����
��һ������ þ������$ (Metagonia)$ �Ĺ����У���$100$�������ͥ��

ÿ�꣬��Щ�����ͥ��Ҫ�յ�������֪֮�׵����ɸ������õ�С���顣��֪��һЩ����С����Ĺ���

1. ���ĳ����һ����ͥ�յ���С���飬��ô�����ͥ���յ���С����ĸ�����������ֻ����$2$��$3$��

2. ���ĳ����һ����ͥ�յ���$a>0$��С���飬ͬ����һ����ͥ�յ���$b>0$��С���飬��ô$a$������$b$��$b$Ҳ������$a$��

���ڣ�����Ϊ��֪֮�ף���֪�����������$t$���У���ÿ���ж��ٸ�С���顣��������Ҫ�ҵ�����һ�����еķ������Ա��ڽ�����$t$�����ܹ����а�������䡣

--------

��һ�У�����һ��������$t(1��t��1000)$��

��������$t$�У�ÿ����һ��������$n_i(1��n_i��10^{18})$����ʾ�ڵ�$i$���У����������֧���С���������

--------

����ÿ��������С���һ��Ӧ����һ����$m_i$,��ʾ�ܹ��յ�С����ļ�ͥ����Ŀ��

�ڶ�����$m_i$������������ÿ����ͥӦ���յ���С����ĸ�������Щ����֮��Ӧ�õ���$n_i$��

---------

ʱ�����ƣ�$2s$

�ռ����ƣ�$256MB$

�����ṩ��@Trexmao

```input1
4
1
2
3
10

```

```output1
1
1
1
2
1
3
2
4 6

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



