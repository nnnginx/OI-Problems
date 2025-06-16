## ��Ŀ����
Farmer John's $N$ cows $(1��N��10^5)$ are spread far apart on his farm and would like to build a communication network so they can more easily exchange electronic text messages (all of which of course contain variations of "moo").

The ith cow is located at a distinct location $(x_i,y_i)$ where $0��x_i��10^6$ and $0��y_i��10$. The cost of building a communication link between cows $i$ and $j$ is the squared distance between them: $(x_i-x_j)^2+(y_i-y_j)^2$.

Please calculate the minimum cost required to build a communication network across which all the cows can communicate. Two cows can communicate if they are directly connected by a link, or if there is a sequence of links along which their message can travel.

**Note: the time limit for this problem is 4s, twice the default.**

## �����ʽ
The first line of input contains $N$, and the next $N$ lines each describe the $x$ and $y$ coordinates of a cow, all integers.

## �����ʽ
Please output the minimum cost of a network that will allow all cows to communicate. Note that this cost might be too large to fit into a 32-bit integer and may require use of 64-bit integers (e.g., "long long" integers in C++).

## ��Ŀ����
## ��Ŀ����


ũ��Լ���� $N$ ͷţ��$1\le N\le10^5$�� ������ũ����ֲ��ļ����Զ�����ϣ���㽨��һ��ͨѶ���磬�������Ǹ����׵ؽ������Ӷ��ţ���Ȼ����Щ���Ŷ����� `moo` �ı����壬�����֣�

�� $i$ ͷţλ��λ�� $(x_i��y_i)$ ���� $0\le x\le 10^6$, $0\le y\le 10$. ��ţ $i$ ��ţ $j$ ֮�佨��ͨ����·�ĳɱ�������֮���ŷ����¾����ƽ������ $(x_i-x_j)^2+(y_i-y_j)^2$


��������㹹��һ��������ţ���ܽ�������ͳɱ���ͨ�����硣�����ͷ��ţͨ��һ������ֱ�����ӻ������ǵ���Ϣ��������һ�����Ӵ�������ô��Ϊ���ǿ���ͨ�š�

#### ע�� ������ʱ������Ϊ4��

## �����ʽ
��һ������Ϊ $N$�������� $N$ �зֱ�������ţ��λ�� $(x,y)$ ��Ϊ����
## �����ʽ
���������������ţͨ�ŵ��������ͳɱ�����ע�⣬�˿�������̫���޷����� 32 λ�����У����ҿ�����Ҫʹ�� 64 λ���������磬C++�еġ�long long������

### ˵��/��ʾ 

���Ե� 2~3 ���� $N\le1000$��

���Ե� 4~15 û���������ơ�

```input1
10
83 10
77 2
93 4
86 6
49 1
62 7
90 3
63 4
40 10
72 0
```

```output1
660
```

## ��ʾ
�����ݷ�Χ��

- Test cases 2-3 satisfy $N��1000$.
- Test cases 4-15 satisfy no additional constraints.

