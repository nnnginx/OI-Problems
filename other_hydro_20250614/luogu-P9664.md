## ��Ŀ����
Given a complete undirected graph of $n$ vertices and $n$ strings $s_1, s_2, \cdots, s_n$, the weight of edge connecting vertices $i$ and $j$ is equal to the length of the longest common substring (LCS) between $s_i$ and $s_j$. Compute the maximum total weight of any spanning tree on this graph.

A substring of a string can be obtained by removing some (possibly zero) characters from the beginning and/or the end of that string. For example, ``maca``, ``aca`` and ``cau`` are all substrings of ``macau``, while ``acu`` is not.

## �����ʽ
There is only one test case in each test file.

The first line of the input contains one integer $n$ ($1 \leq n \leq 2 \times 10^6$) indicating the number of vertices and strings.

For the following $n$ lines, the $i$-th line contains one string $s_i$ ($1 \le |s_i| \le 2 \times 10^6$) consisting only of lowercase English letters.

It's guaranteed that the sum of lengths of all strings will not exceed $2 \times 10^6$.

## �����ʽ
Output one line containing one integer indicating the answer.

## ��Ŀ����
**����Ŀ������**

����һ���� $n$ ���������ȫ����ͼ�� $n$ ���ַ��� $s_1, s_2, \cdots, s_n$�����Ӷ��� $i$ �� $j$ �ıߵ�Ȩ�ص����ַ��� $s_i$ �� $s_j$ ��������Ӵ���LCS���ĳ��ȡ������ͼ�������������������Ȩ�ء�

һ���ַ������Ӵ�����ͨ���Ӹ��ַ����Ŀ�ͷ��/���βɾ��һЩ������Ϊ�㣩�ַ�����á����磬��maca������aca�� �͡�cau�����ǡ�macau�����Ӵ�������acu�����ǡ�

**�������ʽ��**

ÿ�������ļ��а���һ������������

����ĵ�һ�а���һ������ $n$ ($1 \leq n \leq 2 \times 10^6$)����ʾ������ַ�����������

�������� $n$ �У��� $i$ �а���һ���ַ��� $s_i$ ($1 \le |s_i| \le 2 \times 10^6$)����СдӢ����ĸ��ɡ�

��֤�����ַ����ĳ���֮�Ͳ����� $2 \times 10^6$��

**�������ʽ��**

���һ�У�����һ����������ʾ�𰸡�

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
4
icpc
macau
regional
contest
```

```output1
4
```

```input2
3
ababa
babab
aba
```

```output2
7
```

