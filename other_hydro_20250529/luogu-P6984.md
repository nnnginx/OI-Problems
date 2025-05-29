## ��Ŀ����


Louis $L$ Le Roi-Univers has ordered to improve the landscape that is seen from the royal palace. His Majesty prefers to see a high mountain.

The Chief Landscape Manager is going to raise a mountain for Louis. He represents a landscape as a flat picture on a grid of unit squares. Some of the squares are already filled with rock, while others are empty. This greatly simplifies the design. Unit squares are small enough, and the landscape seems to be smooth from the royal palace.

The Chief Landscape Manager has a plan of the landscape -- the heights of all rock-filled columns for each unit of width. He is going to add at most $n$ square units of stones atop of the existing landscape to make a mountain with as high peak as possible. Unfortunately, piles of stones are quite unstable. A unit square of stones may be placed only exactly on top of the other filled square of stones or rock, moreover the squares immediately to the bottom-left and to bottom-right of it should be already filled.

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/11746/1.png)

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/11746/2.png)

Existing landscape

Improved landscape

Your task is to help The Chief Landscape Manager to determine the maximum height of the highest mountain he can build.



## �����ʽ


The first line of the input file contains two integers $w$ -- the width of the existing landscape and $n$ -- the maximum number of squares of stones to add $(1 \le w \le 100 000 , 0 \le n \le 10^{18}).$

Each of the following $w$ lines contains a single integer $h_{i}$ -- the height of the existing landscape column $(1 \le h_{i} \le 10^{9}).$



## �����ʽ


The output file shall contain the single integer -- the maximum possible landscape height after at most $n$ unit squares of stones are added in a stable way.



## ��Ŀ����
�������� $\{h_i\}(i\in[1,w])$ �ͳ��� $n$��

$\forall i\in(1,w)$ ������ $h_{i-1} \geq h_i$ �� $h_{i+1} \geq h_i$ ʱ��ʹ $h_i$ ��Ϊ $h_i+1$ ���Ҳ����������ܶ��� $n$ �Ρ�

�����кϷ������£�$\max\{h_i\}$ �����ֵ��

$1\leq w\leq 10^5,1\leq h_i \leq 10^9,1\leq n\leq 10^{18}.$

```input1
8 4
3
4
2
1
3
3
2
4

```

```output1
5

```

```input2
3 100
3
3
3

```

```output2
4

```

## ��ʾ
Time limit: 1 s, Memory limit: 256 MB. 



