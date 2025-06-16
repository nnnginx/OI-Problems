## ��Ŀ����
You are doing volunteer work for a programming competition in an ancient hotel. Unfortunately, the hotel provides no phone signal or tap water since it can be dated back to the Qin Dynasty, and you have to assign the contestants to the hotel rooms manually instead of using the internet apps. Fortunately, the hotel has sufficient rooms, and you have taken a computer that lets you do some computation locally.

There are $n$ teams, each with exactly $3$ contestants. There are $2$ types of rooms in the hotel, the single room and double room, which can receive at most $1$ and $2$ contestants, respectively. To avoid embarrassing contestants, if two contestants are assigned to a double room, they must come from the same team and have the same gender.

The cost of each room of the same type is the same, but different types may have different costs. Your program needs to calculate the minimum price the host has to pay. The teams are waiting in the registration hall now, and the competition finance officer relies on you to save costs and make a fortune by the residual value. Be quick, or the finance officer will sue you for violating his reputation!

## �����ʽ
The first line of input contains three integers $n$, $c_1$ and $c_2$ ($1 \leq n, c_1, c_2 \leq 1\,000$), denoting the number of teams, the cost of a single room and a double room respectively.

In the following $n$ lines, each line contains a string $S$ with exactly $3$ uppercase English letters. The letters in a string denote the genders of the contestants in one team and will be represented by $\texttt{A}$ to $\texttt{Z}$, respecting the diversity of human beings.

## �����ʽ
The output should contain a single integer, denoting the minimum cost of hotel allocation for contestants.

## ��Ŀ����
### ��Ŀ����

������һ���Ŵ��ľƵ���Ϊһ����̾�����־Ը�������Ƶ����ʷ����׷�ݵ��س������ԾƵ겻�ṩ�ֻ��źź�����ˮ�����޷�ʹ��������������ò��ֶ�Ϊ�����߷��䷿�䡣���˵��ǣ��Ƶ�ӵ�г���ķ��䣬��������һ̨���԰�����һЩ���㡣

���� $n$ �����飬ÿ������ǡ�� $3$ ��ѡ�֡��Ƶ������ַ��䣬���˼��˫�˼䣬�ֱ�������� $1$ �� $2$ ��ѡ�֡�Ϊ�˱���ʹѡ�����Σ��������ѡ�ַ��䵽��ͬһ��˫�˼䣬���Ǳ�������ͬһ�����飬��ӵ����ͬ���Ա�

��ͬ����ķ���Ļ�����ͬ������ͬ����ķ��仨�ѿ��ܲ�ͬ������Ҫ�������췽������Ҫ������Ǯ��ѡ�����Ѿ��ڵǼ����Ⱥ��ʱ������������������������ʡ��֧��˽��ʣ������Ǯ����ơ�����Ҫ����������񣬷���������������ַ�����������Ȩ��

$1\leq n, c_1, c_2\leq 1000$��

### �����ʽ

��һ���������� $n, c_1, c_2$���ֱ��ʾ�������������˼䵥�ۺ�˫�˼䵥�ۡ�

�������� $n$ �У�ÿ��һ������Ϊ $3$ ���ַ��� $S$ ��ʾһ������Ĳ�����Ա���Ա�Ϊ����������Ķ����ԣ�$S$ ���ܰ����� $\texttt A$ �� $\texttt Z$ �����д�д��ĸ��

### �����ʽ

���һ��һ��������ʾ���䷿�����С���ۡ�

```input1
3 1 3
MMM
MMM
FFF

```

```output1
9

```

```input2
3 3 1
ABC
DEF
GHI

```

```output2
9

```

```input3
10 438 438
WWW
SOU
PUN
ETC
OME
CFI
NAL
GOO
DHO
TEL

```

```output3
12264

```

## ��ʾ
**Source**: The 2022 ICPC Asia Xi'an Regional Contest Problem F.

**Author**: fstqwq.

