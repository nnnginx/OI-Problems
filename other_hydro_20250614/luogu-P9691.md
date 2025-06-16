## ��Ŀ����
China Mobile Shenzhen Branch was registered in $1999$. Four years later, Guangdong Collegiate Programming Contest was held for the first time. China Mobile Shenzhen Branch, along with Guangdong Collegiate Programming Contest, witnesses the prosperity and development of the computer industry in Guangdong.

![](https://cdn.luogu.com.cn/upload/image_hosting/md6qj7fz.png)

During the construction of a communication line, it is critical to carefully choose the locations for base stations. The distance from west to east of a city is $n$ kilometers. The engineers have investigated the cost to build a base station at $1, 2, \cdots, n$ kilometers from west to east, which are $a_1, a_2, \cdots, a_n$ respectively.

To ensure communication quality for the residents, the locations of base stations also need to meet $m$ requirements. The $i$-th requirement can be represented as a pair of integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$), indicating that there must be at least $1$ base station between $l_i$ kilometers and $r_i$ kilometers (both inclusive) from west to east.

As the chief engineer, you need to decide the number of base stations to build and their locations, and finally calculate the minimum total cost to satisfy all requirements.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($1 \le n \le 5 \times 10^5$) indicating the distance from west to east of the city.

The second line contains $n$ integers $a_1, a_2, \cdots, a_n$ ($1 \le a_i \le 10^9$) where $a_i$ indicates the cost to build a base station at $i$ kilometers from west to east.

The third line contains an integer $m$ ($1 \le m \le 5 \times 10^5$) indicating the number of requirements.

For the following $m$ lines, the $i$-th line contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) indicating that there must be at least $1$ base station between $l_i$ kilometers and $r_i$ kilometers (both inclusive) from west to east.

It's guaranteed that neither the sum of $n$ nor the sum of $m$ of all test cases will exceed $5 \times 10^5$.

## �����ʽ
For each test case output one line containing one integer indicating the minimum total cost to satisfy all requirements.

## ��Ŀ����
**����Ŀ������**

�й��ƶ�ͨ�ż��Ź㶫���޹�˾���ڷֹ�˾�����¼��``�����ƶ�``���� $1999$ ����ʽע�ᡣ����󣬹㶫ʡ��ѧ��������ƾ�����һ�ξٰ졣�����ƶ���㶫ʡ��ѧ��������ƾ���һ���֤�˹㶫ʡ�������ҵ�������뷢չ��

�ڽ���ͨ����·�Ĺ����У��źŻ�վ��ѡַ��һ���ǳ��ؼ������⡣ĳ���д��������ľ���Ϊ $n$ ǧ�ף�����ʦ���Ѿ��������ڴ������� $1, 2, \cdots, n$ ǧ�׵�λ�ý����վ�ĳɱ����ֱ��� $a_1, a_2, \cdots, a_n$��

Ϊ�˱�֤�����ͨ����������վ��ѡַ����Ҫ���� $m$ �����󡣵� $i$ �����������һ������ $l_i$ �� $r_i$ ��ʾ��$1 \le l_i \le r_i \le n$��������������� $l_i$ ǧ�׵� $r_i$ ǧ�׵�λ��֮�䣨�����ˣ�������Ҫ���� $1$ ����վ��

��Ϊ�ܹ���ʦ������Ҫ������վ��������λ�ã����������������������С�ܳɱ���

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$ ��ʾ������������������ÿ��������ݣ�

��һ������һ������ $n$��$1 \le n \le 5 \times 10^5$����ʾ���д��������ľ��롣

�ڶ������� $n$ ������ $a_1, a_2, \cdots, a_n$��$1 \le a_i \le 10^9$�������� $a_i$ ��ʾ�ڴ������� $i$ ǧ�׵�λ�ý����վ�ĳɱ���

����������һ������ $m$��$1 \le m \le 5 \times 10^5$����ʾ�����������

���ڽ����� $m$ �У��� $i$ �������������� $l_i$ �� $r_i$��$1 \le l_i \le r_i \le n$����ʾ�������� $l_i$ ǧ�׵� $r_i$ ǧ�׵�λ��֮�䣨�����ˣ�������Ҫ���� $1$ ����վ��

��֤�������� $n$ ֮���� $m$ ֮�;������� $5 \times 10^5$��

**�������ʽ��**

ÿ���������һ��һ����������ʾ���������������С�ܳɱ���

**���������͡�**

���ڵ�һ���������ݣ����ŷ������ڴ������� $2$ ǧ�׺� $5$ ǧ�׵�λ�ý����վ���ܳɱ�Ϊ $2 + 100 = 102$��

���ڵڶ����������ݣ����ŷ������ڴ������� $2$ ǧ�׺� $4$ ǧ�׵�λ�ý����վ���ܳɱ�Ϊ $3 + 2 = 5$��

```input1
2
5
3 2 4 1 100
3
1 3
2 4
5 5
5
7 3 4 2 2
3
1 4
2 3
4 5
```

```output1
102
5
```

## ��ʾ
For the first sample test case the optimal solution is to build base stations at $2$ kilometers and $5$ kilometers from west to east. The total cost is $2 + 100 = 102$.

For the second sample test case the optimal solution is to build base stations at $2$ kilometers and $4$ kilometers from west to east. The total cost is $3 + 2 = 5$.

