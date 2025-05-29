## ��Ŀ����
BaoBao has just found a grid with $n$ rows and $m$ columns in his left pocket, where the cell in the $j$-th column of the $i$-th row (indicated by $(i, j)$) contains an arrow (pointing either upwards, downwards, leftwards or rightwards) and an integer $a_{i, j}$.

BaoBao decides to play a game with the grid. He will first select a cell as the initial cell and tick it. After ticking a cell (let's say BaoBao has just ticked cell $(i, j)$), BaoBao will go on ticking another cell according to the arrow and the integer in cell $(i, j)$.

- If the arrow in cell $(i, j)$ points upwards, BaoBao will go on ticking cell $(i-a_{i, j}, j)$ if it exists.
- If the arrow in cell $(i, j)$ points downwards, BaoBao will go on ticking cell $(i+a_{i, j}, j)$ if it exists.
- If the arrow in cell $(i, j)$ points leftwards, BaoBao will go on ticking cell $(i, j-a_{i, j})$ if it exists.
- If the arrow in cell $(i, j)$ points rightwards, BaoBao will go on ticking cell $(i, j+a_{i, j})$ if it exists.

If the cell BaoBao decides to tick does not exist, or if the cell is already ticked, the game ends.

BaoBao is wondering if he can select a proper initial cell, so that he can tick every cell in the grid exactly once before the game ends. Please help him find the answer.


## �����ʽ
There are multiple test cases. The first line contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($1 \le n \times m \le 10^5$), indicating the number of rows and columns of the grid.

For the following $n$ lines, the $i$-th line contains a string $s_i$ consisting of lowercased English letters ($|s_i| = m$, $s_{i, j} \in \{\text{`u' (ascii: 117)}, \text{`d' (ascii: 100)}, \text{`l' (ascii: 108)}, \text{`r'(ascii: 114)}\}$), where $s_{i, j}$ indicates the direction of arrow in cell $(i, j)$.

- If $s_{i, j} = \text{`u'}$, the arrow in cell $(i, j)$ points upwards.
- If $s_{i, j} = \text{`d'}$, the arrow in cell $(i, j)$ points downwards.
- If $s_{i, j} = \text{`l'}$, the arrow in cell $(i, j)$ points leftwards.
- If $s_{i, j} = \text{`r'}$, the arrow in cell $(i, j)$ points rightwards.

For the following $n$ lines, the $i$-th line contains $m$ integers $a_{i, 1}, a_{i, 2}, \dots, a_{i, m}$ ($1 \le a_{i, j} \le \max(n, m)$), where $a_{i, j}$ indicates the integer in cell $(i, j)$.

It's guaranteed that the sum of $n \times m$ of all test cases does not exceed $10^6$.

## �����ʽ
For each test case output one line. If BaoBao can find a proper initial cell, print ``Yes`` (without quotes), otherwise print ``No`` (without quotes).


## ��Ŀ����
**����Ŀ������**

�����ո���������ڴ��﷢����һ�� $n$ �� $m$ �е��������е� $i$ �е� $j$ �еĵ�Ԫ�񣨱�ʾΪ $(i, j)$������һ����ͷ��ָ���ϡ��¡�����ң���һ������ $a_{i, j}$��

�������������������һ����Ϸ�������Ȼ�ѡ��һ����Ԫ����Ϊ��ʼ��Ԫ�񲢱�������ڱ��һ����Ԫ��֮�󣨼��豦���ոձ���˵�Ԫ�� $(i, j)$�������������ݵ�Ԫ�� $(i, j)$ �еļ�ͷ���������������һ����Ԫ��

- �����Ԫ�� $(i, j)$ �еļ�ͷָ���Ϸ���������������ǵ�Ԫ�� $(i-a_{i, j}, j)$������õ�Ԫ����ڵĻ���
- �����Ԫ�� $(i, j)$ �еļ�ͷָ���·���������������ǵ�Ԫ�� $(i+a_{i, j}, j)$������õ�Ԫ����ڵĻ���
- �����Ԫ�� $(i, j)$ �еļ�ͷָ���󷽣�������������ǵ�Ԫ�� $(i, j-a_{i, j})$������õ�Ԫ����ڵĻ���
- �����Ԫ�� $(i, j)$ �еļ�ͷָ���ҷ���������������ǵ�Ԫ�� $(i, j+a_{i, j})$������õ�Ԫ����ڵĻ���
�������������ǵĵ�Ԫ�񲻴��ڣ����߸õ�Ԫ���Ѿ�����ǣ���Ϸ������

������֪�����Ƿ����ѡ��һ�����ʵĳ�ʼ��Ԫ���Ա�����Ϸ����ǰǡ�ñ�������е�ÿһ����Ԫ��һ�Ρ���������ҵ��𰸡�

**�������ʽ��**

�ж��������������һ�а���һ������ $T$����ʾ��������������������ÿ������������

��һ�а����������� $n$ �� $m$ ($1 \le n \times m \le 10^5$)����ʾ�����������������

�������� $n$ ���У��� $i$ �а���һ���ַ��� $s_i$����СдӢ����ĸ��ɣ�$|s_i| = m$��$s_{i, j} \in \{\text{`u' (ascii: 117)}, \text{`d' (ascii: 100)}, \text{`l' (ascii: 108)}, \text{`r'(ascii: 114)}\}$�������� $s_{i, j}$ ��ʾ��Ԫ�� $(i, j)$ �м�ͷ�ķ���

- ��� $s_{i, j} = \text{`u'}$����Ԫ�� $(i, j)$ �еļ�ͷָ���Ϸ���
- ��� $s_{i, j} = \text{`d'}$����Ԫ�� $(i, j)$ �еļ�ͷָ���·���
- ��� $s_{i, j} = \text{`l'}$����Ԫ�� $(i, j)$ �еļ�ͷָ���󷽡�
- ��� $s_{i, j} = \text{`r'}$����Ԫ�� $(i, j)$ �еļ�ͷָ���ҷ���

�������� $n$ ���У��� $i$ �а��� $m$ ������ $a_{i, 1}, a_{i, 2}, \dots, a_{i, m}$ ($1 \le a_{i, j} \le \max(n, m)$)������ $a_{i, j}$ ��ʾ��Ԫ�� $(i, j)$ �е�������

��֤���в��������� $n \times m$ ֮�Ͳ����� $10^6$��

**�������ʽ��**

����ÿ�������������һ�С�������������ҵ�һ�����ʵĳ�ʼ��Ԫ����� ��Yes�����������ţ���������� ��No�����������ţ���

**���������͡�**

���ڵ�һ��ʾ��������������������ѡ��Ԫ�� $(1, 2)$ ��Ϊ��ʼ��Ԫ�����������԰�����˳��ǡ�ô����е�Ԫ��$(1, 2), (2, 2), (2, 3), (2, 1), (1, 1), (1, 3)$��

���ڵڶ���ʾ����������������ѡ���ĸ���Ԫ����Ϊ��ʼ��Ԫ�񣬱������ֻ�ܴ� 2 ����Ԫ��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
2
2 3
rdd
url
2 1 1
1 1 2
2 2
rr
rr
1 1
1 1
```

```output1
Yes
No
```

## ��ʾ
For the first sample test case, BaoBao can select cell $(1, 2)$ as the initial cell, so that he can tick all the cells exactly once in the following order: $(1, 2), (2, 2), (2, 3), (2, 1), (1, 1), (1, 3)$.

For the second sample test case, BaoBao can only tick at most $2$ cells no matter which cell is selected as the initial cell.


