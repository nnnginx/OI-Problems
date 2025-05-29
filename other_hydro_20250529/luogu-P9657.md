## ��Ŀ����
As the leader of the safety department, you are asked to check an ancient matching system in your company. 

The system is fed with two strings, a to-be-matched string and a pattern string, and will determine whether the former can match the latter. The former string is a strict binary string(i.e., contains only $\textbf{0}$ and $\textbf{1}$), and the latter string consists of four types of characters $\textbf{0}$, $\textbf{1}$, $\textbf{*}$, $^$, where $\textbf{*}$ means match zero or more arbitrary binary characters, and $^$ means match exactly one binary character. 

The system has two matching methods: maximum matching and minimum matching.

Consider the starting positions of the two strings. The maximum matching method will make different decisions based on the current character of the pattern string:
- $\textbf{*}$: The system will enumerate $i$ from $L$ to $0$, where $L$ is the remaining length of the to-be-matched string. Before each enumeration starts, the system consumes 1 unit of energy. Then it temporarily assumes that the current $\textbf{*}$ in the pattern string matches the consecutive $i$ characters in the to-be-matched string, and tries to match the remaining positions of two strings recursively. As long as one attempt is successful, the system will give up the remaining enumeration and stop the whole system. Otherwise, it will try the next enumeration until all attempts are tried and finally return to the previous $\textbf{*}$ enumeration.
- $\textbf{0,1}$: The system will stop and return to the previous $\textbf{*}$ enumeration if the to-be-matched string has been exhausted. Otherwise, it consumes $1$ unit of energy to compare the current characters between the pattern string and the to-be-matched string. It will continue analyzing the remaining positions of these two strings if the result is the same, otherwise, return back to the previous $\textbf{*}$ enumeration.
- $^$: The system will stop and return to the previous $\textbf{*}$ enumeration if the to-be-matched string has been exhausted. Otherwise, it consumes $1$ unit of energy and moves on of two strings.

When the pattern string is exhausted, the system will check the to-be-matched string at the same time. It will return ``Yes`` and stop the whole process if the to-be-matched string is also exhausted, otherwise, it will return to the previous $\textbf{*}$ enumeration. After all attempts are tried and no matching method is found, the system will eventually return ``No``.

Minimum matching does a similar thing except for the enumeration order of $\textbf{*}$ (i.e., enumerate $i$ from $0$ to $L$).

These two matching methods seem not very effective, so you want to hack them. Please construct both a pattern string and a to-be-matched string of length $n$ for each matching method, so that the system answers ``Yes`` and the energy consumption is as large as possible.


## �����ʽ
There is only one test case in each test file.

The first and only line contains an integer $n$ ($1 \le n \le 10^3$) indicating the length of strings need to be constructed.

## �����ʽ
Please output the pattern string, the to-be-matched string, and the energy cost for the maximum matching method in the first $3$ lines. Then output the pattern string, the to-be-matched string, and the energy cost for the minimum matching method in the next $3$ lines.

If there are multiple constructing ways, you can output any of them.

The energy cost may be very large, so you need to output the value modulo $(10^9+7)$. Note that this is only for your convenience and you need to maximize the energy cost before the modulus.

```input1
3
```

```output1
*0*
011
8
**1
101
7
```

## ��ʾ
**����Ŀ������**

��Ϊ��ȫ���ŵĸ����ˣ��㱻Ҫ���鹫˾��һ������ƥ��ϵͳ��

��ϵͳ���������ַ�����һ����ƥ���ַ�����һ��ģʽ�ַ�������ȷ��ǰ���Ƿ���ƥ����ߡ�ǰ���ַ������ϸ�Ķ������ַ������������� $\textbf{0}$ �� $\textbf{1}$�����������ַ������������͵��ַ���� $\textbf{0}$��$\textbf{1}$��$\textbf{*}$ �� $^$������ $\textbf{*}$ ��ʾƥ�������������������ַ���$^$ ��ʾƥ��ǡ��һ���������ַ���

��ϵͳ������ƥ�䷽�������ƥ�����Сƥ�䡣

���������ַ�������ʼλ�á����ƥ�䷽��������ģʽ�ַ����ĵ�ǰ�ַ�������ͬ�ľ�����
- $\textbf{*}$: ϵͳ���� $L$ �� $0$ ö�� $i$������ $L$ �Ǵ�ƥ���ַ�����ʣ�೤�ȡ���ÿ��ö�ٿ�ʼ֮ǰ��ϵͳ���� 1 ��λ��������Ȼ������ʱ����ģʽ�ַ����еĵ�ǰ $\textbf{*}$ ƥ���ƥ���ַ����е����� $i$ ���ַ��������Եݹ��ƥ�������ַ�����ʣ��λ�á�ֻҪ��һ�γ��Գɹ���ϵͳ������ʣ���ö�ٲ�ֹͣ����ϵͳ����������������һ��ö�٣�ֱ�����г��Զ�������ϣ���󷵻ص���ǰ�� $\textbf{*}$ ö�١�
- $\textbf{0,1}$: �����ƥ���ַ����Ѿ��ľ�����ϵͳ��ֹͣ�����ص���ǰ�� $\textbf{*}$ ö�١������������� $1$ ��λ���������Ƚ�ģʽ�ַ����ʹ�ƥ���ַ���֮��ĵ�ǰ�ַ�����������ͬ���������������������ַ�����ʣ��λ�ã����򣬷��ص���ǰ�� $\textbf{*}$ ö�١�
- $^$: �����ƥ���ַ����Ѿ��ľ�����ϵͳ��ֹͣ�����ص���ǰ�� $\textbf{*}$ ö�١������������� $1$ ��λ���������������������ַ�����

��ģʽ�ַ����ľ�ʱ��ϵͳ��ͬʱ����ƥ���ַ����������ƥ���ַ���Ҳ�Ѿ��ľ�����ϵͳ�����ء��ǡ���ֹͣ�������̣������������ص���ǰ�� $\textbf{*}$ ö�١��ڳ��������г��Բ��Ҳ���ƥ�䷽����ϵͳ���ս����ء��񡱡�

��Сƥ��ִ�����ƵĲ��������� $\textbf{*}$ ��ö��˳�򣨼��� $0$ �� $L$ ö�� $i$����

������ƥ�䷽���ƺ���̫��Ч����������ڵ����ǡ���Ϊÿ��ƥ�䷽������һ������Ϊ $n$ ��ģʽ�ַ����ʹ�ƥ���ַ�����ʹ��ϵͳ���ء��ǡ����������ľ����ܴ�

**�������ʽ��**

ÿ�������ļ���ֻ��һ������������

��һ�н�����һ������ $n$��$1 \le n \le 10^3$������ʾ��Ҫ������ַ����ĳ��ȡ�

��������ƥ�䷽����ģʽ�ַ�������ƥ���ַ������������ĵ�ǰ $3$ �С�Ȼ�������Сƥ�䷽����ģʽ�ַ�������ƥ���ַ������������ĵĺ� $3$ �С�

**�������ʽ��**

����ж��ֹ��췽ʽ�����������κ�һ�֡�

�������Ŀ��ܷǳ�����������Ҫ���ȡģ $(10^9+7)$ ���ֵ����ע�⣬����������㣬����Ҫ��ȡģ֮ǰ����������ġ�

���������ڣ�[ChatGPT](https://chatgpt.com/)��

