## ��Ŀ����
Prof. Pang invited $n$ professors to his banquet. The professors sit at a round table. For all $i$ from $1$ to $n$, professor $i$ sits adjacent to professor $(i \bmod n) + 1$ and $((i + n - 2)\bmod n) + 1$.

Prof. Pang prepared $n$ dishes. There are $n$ positions on the table. Position $i$ is in front of professor $i$. Professor $i$ can access only the dishes placed at positions $i$, $(i \bmod n) + 1$, and $((i + n - 2)\bmod n) + 1$. Prof. Pang will place exactly one dish at each position.

Among the dishes, $a$ of them are spicy and $n-a$ of them are not spicy. Some (possibly $0$) professors are unable to have spicy food. If a professor can have spicy food, his/her **satisfaction level** is the number of dishes (no matter spicy or not) he/she can access. If a professor cannot have spicy food, his/her satisfaction level is the number of not spicy dishes he/she can access.

Prof. Pang knows whether each professor can have spicy food or not. Please help him to arrange the dishes on the table so that the sum of satisfaction levels over all the professors is maximized. Output the maximum sum.

## �����ʽ
The first line contains two integers $n, a$ ($3\le n\le 10^5, 0\le a\le n$). 

The second line contains $n$ integers $b_1, \ldots, b_n$. $b_i$ is $0$ or $1$. $b_i=1$ means professor $i$ can have spicy food. $b_i=0$ means professor $i$ cannot have spicy food.

## �����ʽ
Output one integer representing the answer in one line.

## ��Ŀ����
**����Ŀ������**

�ӽ��������� $n$ λ���ڲμ�������ᡣ����������һ��Բ����Χ���������� $i$���� $1$ �� $n$������ $i$ ���ڽ��� $(i \bmod n) + 1$ �� $((i + n - 2)\bmod n) + 1$ �Աߡ�

�ӽ���׼���� $n$ ���ˡ��������� $n$ ��λ�á�λ�� $i$ �ڽ��� $i$ ��ǰ�档���� $i$ ֻ�ܽӴ�������λ�� $i$��$(i \bmod n) + 1$ �� $((i + n - 2)\bmod n) + 1$ ���Ĳˡ��ӽ��ڽ���ÿ��λ���Ϸ���һ���ˡ�

����Щ���У��� $a$ �������ģ�$n-a$ ���ǲ����ġ���Щ������Ϊ $0$�����ڲ��ܳ�����ʳ����һλ���ڿ��Գ�����ʳ���/����**�����ˮƽ**����/�����ԽӴ����Ĳ˵����������������Ļ��ǲ����ģ������һλ���ڲ��ܳ�����ʳ���/���������ˮƽ����/�����ԽӴ����Ĳ����Ĳ˵�������

�ӽ���֪��ÿλ�����Ƿ���Գ�����ʳ�����������������ϵĲˣ�ʹ�����н��ڵ������ˮƽ֮����󻯡���������ܺ͡�

**�������ʽ��**

��һ�а����������� $n, a$ ($3\le n\le 10^5, 0\le a\le n$)��

�ڶ��а��� $n$ ������ $b_1, \ldots, b_n$��$b_i$ �� $0$ �� $1$��$b_i=1$ ��ʾ���� $i$ ���Գ�����ʳ�$b_i=0$ ��ʾ���� $i$ ���ܳ�����ʳ�

**�������ʽ��**

���һ��һ����������ʾ�𰸡�

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
5 2
1 0 1 0 1

```

```output1
13

```

