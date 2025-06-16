## ��Ŀ����
It's already 21:30 now, and it's time for BaoBao to go to bed. To ensure his sleeping quality, BaoBao decides to turn all the lights in his bedroom off.

There are $n$ lights, numbered from 1 to $n$, arranged in a row in BaoBao's bedroom. Each time BaoBao can select an integer $i$ and turn all the lights numbered from $i$ to $(i+L-1)$ (both inclusive) off, where $L$ is a predefined positive integer. Note that each time the value of $L$ must be the same.

Given the initial status of all the lights, please help BaoBao determine the smallest possible $L$ so that he can turn all the lights off within $k$ times.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \times 10^5$).

The second line contains a string $s$ ($|s| = n$, $s \in \{\text{`0'}, \text{`1'}\}$) indicating the initial status of the lights. Let $s_i$ be the $i$-th character in $s$, if $s_i = \text{`1'}$ then the $i$-th light is initially on, otherwise it's initially off. It's guaranteed that there is at least one `1�� in $s$.

It's guaranteed that the sum of $n$ of all test cases will not exceed $2 \times 10^6$.

## �����ʽ
For each test case output one line containing one integer, indicating the smallest possible $L$.

## ��Ŀ����
**����Ŀ������**

�����Ѿ��� 21:30 �ˣ��������ϴ�˯���ˡ�Ϊ��ȷ������˯�����������������ص�����������еơ�

�������������� $n$ յ�ƣ���1�� $n$ �ų�һ�š�ÿ�α�������ѡ��һ������ $i$�������ӵ� $i$ յ�Ƶ��� $(i+L-1)$ յ�ƣ��������ˣ�֮������еƹص������� $L$ ��һ��Ԥ�������������ע�⣬ÿ�β����� $L$ ֵ������ͬ��

�������еƵĳ�ʼ״̬�����������ȷ�����ܵ���С $L$ ʹ�������� $k$ �β����ڹص����еĵơ�


**�������ʽ��**

�ж����������������ĵ�һ�а���һ������ $T$����ʾ��������������������ÿ������������

��һ�а����������� $n$ �� $k$��$1 \le k \le n \le 2 \times 10^5$����

�ڶ��а���һ���ַ��� $s$��$|s| = n$, $s \in \{\text{`0'}, \text{`1'}\}$����ʾ�Ƶĳ�ʼ״̬���� $s_i$ Ϊ�ַ��� $s$ �ĵ� $i$ ���ַ������ $s_i = \text{`1'}$����� $i$ յ�Ƴ�ʼ�����ģ���������ġ���֤ $s$ ��������һ�� `1`��

��֤���в��������� $n$ ֮�Ͳ����� $2 \times 10^6$��

**�������ʽ��**

����ÿ�������������һ�У�����һ����������ʾ���ܵ���С $L$��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
2
10 4
0101011111
3 1
010
```

```output1
3
1
```

