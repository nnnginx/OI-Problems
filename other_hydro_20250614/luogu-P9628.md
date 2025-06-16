## ��Ŀ����
$\textit{Go}$ is an adversarial game with the objective of surrounding a larger total area of the board with one's stones than the opponent's. The core idea of the game is the concept of $\textit{liberty}$, which is an open point, or rather, an intersection of vertical and horizontal lines on the chessboard with no stones on it, bordering the group.

A stone, white or black, is called $\textit{alive}$ if it has at least one liberty directly orthogonally adjacent (up, down, left, or right), or must be in the same connected group with a stone of the same color which is alive. We say two stones of the same color are directly connected if they're orthogonally adjacent. We say two stones $s_1$ and $s_k$ of the same color are in the same connected group if there exists a sequence of stones $s_1, s_2,\cdots, s_k$ such that for all $1 \le i < k$, $s_{i-1}$ and $s_i$ are of the same color and are directly connected.

For example, in the left part of the below figure, neither of the two white stones is alive, as they're captured by the surrounding black stones; While in the right part, the rightmost white stone is also not alive, even if the leftmost black stone is also not alive.

![](https://cdn.luogu.com.cn/upload/image_hosting/zjm3icu0.png)

Given a chessboard with $n$ vertical and $n$ horizontal lines where some stones might be lying on, please calculate the number of white stones captured by the black ones (that is to say, calcaulate the number of white stones not alive). The results for the above examples are $2$ and $1$, respectively.

However, our dear friend Kotori thinks that this problem is too simple for our clever contestants to solve, so she would like to heat things up by instead asking you to flip the color of each stone (that is to say, change a black stone to a white one, or vice versa$^1$) independently and find out the corresponding answer after each flip.

By flipping independently we mean that before flipping the color of a stone, the other stones should change back to their original color. Also note that the data in this problem is not from the real world, which means that the size of the chessboard is not necesssarily $19 \times 19$, and the number of white and black stones can be any integer.

$^1$ Vice versa: The reverse is also true. Here it can be replaced with ``change a white stone to a black one``. This is a very common phrase in modern English especially in academic writing, so please bear it in mind.


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains one integer $n$ ($2\le n \le 10^3$) indicating the length of the board side.

For the next $n$ lines, the $i$-th line contains a string $s_{i,1},s_{i,2},\cdots,s_{i,n}$ ($s_{i,j}$ $\in$ $\{\text{`x' (ascii: 120)}$, $\text{`o' (ascii: 111)}$, $\text{`.' (ascii: 46)}\}$), where $s_{i,j} = \text{`x'}$ indicates that the intersection on the $i$-th row and the $j$-th column contains a black stone. Similarly $s_{i, j} = \text{`o'}$ for a white stone and $s_{i,j} = \text{`.'}$ for an empty intersection.

It's guaranteed that the sum of $n$ over all test cases does not exceed $5 \times 10^3$.

## �����ʽ
For each test case output an integer $E$ modulo $(10^9 + 7)$ which is the answer encoded as follows:
- Sort all the stones with their row number (from top to bottom) as the primary sort key and their column number (from left to right) as the secondary sort key;
- $E=\sum \limits_{i=1}^m (10^6 + 7)^{m-i}a_i$, where $m$ is the number of stones and $a_i$ is the number of white stones not alive after flipping the color of the $i$-th stone.

$\underline{\text{NOTE that the MODULUS and the BASE are} \textbf{ DIFFERENT}}$. (We're begging you to notice this sentence. If this is not a pdf file I would rather it flashes and twinkles like crazy.)


## ��Ŀ����
### ��Ŀ����

**Χ��**��һ�ֶԿ�����Ϸ��Ŀ�������Լ���ʯͷ�ȶ��ֵ�ʯͷ��Χ������������������Ϸ�ĺ���������**����**����һ�����ŵ㣬���߸�ȷ�е�˵���������ϴ�ֱ�ߺ�ˮƽ�ߵĽ���㣬����û��ʯͷ����Ⱥ�������

һ����ɫ���ɫ��ʯͷ�������������һ��ֱ���������ڵ����ɣ��ϡ��¡�����ң������߱�����һ������������ͬ��ɫ��ʯͷ��ͬһ���������У���ô�����������ģ�����Ϊ**����**������˵�����������ɫ��ͬ��ʯͷ�������ڣ����Ǿ�ֱ���������������һϵ��ʯͷ $s_1,s_2,��,s_k$ ���������� $1\leq i<k$ �� $s_{i-1}$ �� $s_i$ ��ɫ��ͬ���������ڣ�����ͬ��ɫ������ʯͷ $s_1$ �� $s_k$ ����ͬһ��ͨ�顣

���磬����ͼ����࣬�����ɫ��ʯͷ��û�л��ţ���Ϊ���Ǳ���Χ�ĺ�ɫʯͷ�����ˣ������ұߵĲ��֣����ұߵİ�ɫʯͷҲû����������ʹ����ߵĺ�ɫʯͷҲû�С�

![Go](https://cdn.luogu.com.cn/upload/image_hosting/zjm3icu0.png)

����һ���� $n$ ����ֱ�ߺ� $n$ ��ˮƽ�ߵ����̣����п�����һЩʯͷ�������棬������ɫʯͷ����İ�ɫʯͷ��������Ҳ����˵������û�������İ�ɫʯͷ���������������ӵĽ���ֱ�Ϊ $2$ �� $1$ ��

Ȼ���������װ������� Kotori ��Ϊ������������Ǵ����Ĳ����߽��̫���ˣ������������������תÿ��ʯͷ����ɫ��Ҳ����˵���Ѻ�ɫ��ʯͷ��ɰ�ɫ��ʯͷ����֮��Ȼ$^1$��������ÿ�η�ת���ҵ���Ӧ�Ĵ𰸡�

������ת����˼�ǣ��ڷ�תʯͷ����ɫ֮ǰ������ʯͷӦ�ñ��ԭ������ɫ����Ҫע�⣬��������е����ݲ���������ʵ���磬����ζ�����̵Ĵ�С��һ���� $19��19$ ���ڰ�ʯͷ����������������������

$^1$��֮��Ȼ��������������� ```�Ѱ�ɫ��ʯͷ��ɺ�ɫ��ʯͷ``` �����档�����ִ�Ӣ���зǳ������Ķ����������ѧ��д���У��������ס��

### �����ʽ

�ж����������������ĵ�һ�а���һ������ $T$ ��ʾ��������������������ÿ������������

��һ�а���һ������ $n$ ($2\leq n\leq 10^3$)����ʾ���̵ı߳���

���ڽ����� $n$ �У��� $i$ �а���һ���ַ��� $s_{i,1},s_{i,2},��,s_{i,n}$ ������ $s_{i,j}=��x��$ ��ʾ�� $i$ �е� $j$ ����һ����ʯͷ��$s_{i,j}=��o��$ ��ʾ�� $i$ �е� $j$ ����һ����ʯͷ��$s_{i,j}=��.��$ ��ʾ�� $i$ �е� $j$ ���ǿյġ�

��֤���в��������� $n$ ֮�Ͳ����� $5��10^3$ ��

### �����ʽ

����ÿ�������������һ������ $E\bmod10^9+7$ ��Ϊ���±���Ĵ𰸣�

- ������ʯͷ�������������кţ����ϵ��£�Ϊ��һ�ؼ��֣������кţ������ң�Ϊ�ڶ��ؼ��֣�
- $E=\sum\limits_{i=1}^m(10^6+7)^{m-i}a_i$ ������ $m$ ��ʯͷ�������� $a_i$ �Ƿ�ת�� $i$ ����ɫ��û�������İ�ɫʯͷ��������

$\underline{\textbf{ע��}\text{��\textsf{ģ��}��\textsf{����}��}\textbf{��ͬ}{��}}$ �������ǿ�����ע����仰������ⲻ�� pdf �ļ�������Ը�������һ����˸����

### ˵��/��ʾ

���ڵڶ����������������� $(1,2),(2,1),(2,2),(2,3),(3,1),(3,2)$ ��˳��תʯͷ�������İ�ɫʯͷ�����ֱ�Ϊ $1,0,1,2,0,0$ ��

���ڵ��������������������ϵ�����ʯͷ�������Ǻ�ɫ���ǰ�ɫ�������ǻ��ŵġ�

```input1
3
2
.o
..
3
.x.
xoo
ox.
2
oo
oo
```

```output1
0
870527216
485539347
```

## ��ʾ
For the second sample test case, after flipping the stones in the order of $(1,2)$, $(2,1)$, $(2,2)$, $(2,3)$, $(3,1)$, $(3,2)$, the number of dead white stones are $1$, $0$, $1$, $2$, $0$, $0$, repectively.

For the third sample test case all stones on the chessboard, black or white, are not alive.

