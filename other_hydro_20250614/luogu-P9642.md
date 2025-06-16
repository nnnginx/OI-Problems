## ��Ŀ����
We call a string as a 0689-string if this string only consists of digits `0`, `6`, `8` and `9`. Given a 0689-string $s$ of length $n$, one $\textbf{must}$ do the following operation exactly once: select a non-empty substring of $s$ and rotate it 180 degrees.

More formally, let $s_i$ be the $i$-th character in string $s$. After rotating the substring starting from $s_l$ and ending at $s_r$ 180 degrees ($1 \le l \le r \le n$), string $s$ will become string $t$ of length $n$ extracted from the following equation, where $t_i$ indicates the $i$-th character in string $t$:

$$t_i = \begin{cases}
s_i & \text{if } 1 \le i < l \text{ or } r < i \le n \\
\text{`0'} & \text{if } l \le i \le r \text{ and } s_{l+r-i} = \text{`0'} \\
\text{`6'} & \text{if } l \le i \le r \text{ and } s_{l+r-i} = \text{`9'} \\
\text{`8'} & \text{if } l \le i \le r \text{ and } s_{l+r-i} = \text{`8'} \\
\text{`9'} & \text{if } l \le i \le r \text{ and } s_{l+r-i} = \text{`6'} \\
\end{cases}$$

What's the number of different strings one can get after the operation?

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first and only line contains a 0689-string $s$ ($1 \le |s| \le 10^6$).

It's guaranteed that the sum of $|s|$ of all test cases will not exceed $10^7$.


## �����ʽ
For each test case output one line containing one integer, indicating the number of different strings one can get after applying the operation exactly once.

## ��Ŀ����
**����Ŀ������**

���ǳ�һ���ַ���Ϊ 0689-�ַ������������ַ���ֻ�������� 0��6��8 �� 9������һ������Ϊ $n$ �� 0689-�ַ��� $s$������ִ�����²���һ�Σ�ѡ�� $s$ ��һ���ǿ��Ӵ���������ת 180 �ȡ�

����ʽ��˵���� $s_i$ Ϊ�ַ��� $s$ �ĵ� $i$ ���ַ����ڽ��� $s_l$ ��ʼ�� $s_r$ �������Ӵ���ת180�Ⱥ� ($1 \le l \le r \le n$)���ַ��� $s$ ����ɳ���Ϊ $n$ ���ַ��� $t$����ͨ�����¹�ʽ�õ������� $t_i$ ��ʾ�ַ��� $t$ �еĵ� $i$ ���ַ���

$$t_i = \begin{cases}
s_i & \text{if } 1 \le i < l \text{ or } r < i \le n \\
\text{`0'} & \text{if } l \le i \le r \text{ and } s_{l+r-i} = \text{`0'} \\
\text{`6'} & \text{if } l \le i \le r \text{ and } s_{l+r-i} = \text{`9'} \\
\text{`8'} & \text{if } l \le i \le r \text{ and } s_{l+r-i} = \text{`8'} \\
\text{`9'} & \text{if } l \le i \le r \text{ and } s_{l+r-i} = \text{`6'} \\
\end{cases}$$

������������󣬿��Եõ����ٸ���ͬ���ַ�����

**�������ʽ��**

�ж����������������ĵ�һ�а���һ������ $T$����ʾ��������������������ÿ������������
- ��һ����Ψһһ�а���һ�� 0689-�ַ��� $s$ ($1 \le |s| \le 10^6$)��
��֤���в��������� $|s|$ ֮�Ͳ����� $10^7$��

**�������ʽ��**

����ÿ�������������һ�У�����һ����������ʾ����һ�β������Եõ��Ĳ�ͬ�ַ�����������

**���������͡�**

�����ڴ˽��͵�һ����������������
$$\begin{array}{|c|c||c|c|}\hline \textbf{�Ӵ�} & \textbf{���} & \textbf{�Ӵ�} & \textbf{���} \\ \hline 0 & 0689 & 68 & 0899 \\ \hline 6 & 0989 & 89 & 0668 \\ \hline 8 & 0689 & 068 & 8909 \\ \hline 9 & 0686 & 689 & 0689 \\ \hline 06 & 9089 & 0689 & 6890 \\ \hline \end{array}$$
�����׷��֣���������������Եõ� 8 ����ͬ���ַ�����

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
2
0689
08
```

```output1
8
2
```

## ��ʾ
We hereby explain the first sample test case.

$$\begin{array}{|c|c||c|c|}\hline \textbf{Substring} & \textbf{Result} & \textbf{Substring} & \textbf{Result} \\ \hline 0 & 0689 & 68 & 0899 \\ \hline 6 & 0989 & 89 & 0668 \\ \hline 8 & 0689 & 068 & 8909 \\ \hline 9 & 0686 & 689 & 0689 \\ \hline 06 & 9089 & 0689 & 6890 \\ \hline \end{array}$$

It's easy to discover that we can get $8$ different strings after the operation.

