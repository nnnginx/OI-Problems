## ��Ŀ����
Rebecca is a tour guide and is trying to market the Rocky Mountains for her magazine. She recently took a beautiful picture consisting of $N$ mountains where the $i\text{-th}$ mountain from the left has a height $h_i$. She will crop this picture for her magazine, by possibly removing some mountains from the left side of the picture and possibly removing some mountains from the right side of the picture. That is, a crop consists of consecutive mountains starting from the $l\text{-th}$ to the $r\text{-th}$ mountain where $l \leq r$. To please her magazine readers, Rebecca will try to find the most symmetric crop.

We will measure the $asymmetric\ value$ of a crop as the sum of the absolute difference for every pair of mountains equidistant from the midpoint of the crop. To help understand that definition, note that the absolute value of $a$ number $v$, written as $|v|$, is the non-negative value of v: for example $\lvert -6 \rvert = 6$ and $|14| = 14$. The asymmetric value of a crop is the sum of all $|h_{l+i} - h_{r-i}|$ for $0 \leq i \leq \frac{r-l}{2}$. To put that formula in a different way, we pair up the mountains working from the outside in toward the centre, calculate the absolute difference in height of each of these pairs, and sum them up.

Because Rebecca does not know how wide the picture needs to be, for all possible crop lengths, find the asymmetric value of the most symmetric crop (the crop with the minimum asymmetric value).

## �����ʽ
The first line consists of an integer $N$, representing the number of mountains in the picture.

The second line consists of $N$ space-separated integers, where the $i\text{-th}$ integer from the left represents $h_i$.

The following table shows how the available 15 marks are distributed:

| Marks | Bounds on $N$ | Bounds on $h_i$ | Additional Constraints |
| :-----------: | :-----------: | :-----------: | :-----------: |
| $5$ | $1 \leq N \leq 300$ | $0 \leq h_i \leq 10^5$ | None. |
| $5$ | $1 \leq N \leq 5000$ | $0 \leq h_i \leq 10^5$ | Height of mountains are in non-decreasing order from left to right. |
| $5$ | $1 \leq N \leq 5000$ | $0 \leq h_i \leq 10^5$ | None. |


## �����ʽ
Output on one line $N$ space-separated integers, where the $i\text{-th}$ integer from the left is the asymmetric value of the most symmetric picture of crops of length $i$.

## ��Ŀ����
Rebecca ��һ�����ɽ������Ƭ������������ $N(1\leq N \leq 5000)$ ��ɽ���������ҵĵ� $i$ ��ɽ�ĸ߶��� $h_i(1\leq h_i \leq 10^5)$��Rebecca ��ͼ������Ƭ��һ�������Σ����Ž�ͼ�Ĳ��Գ��Զ���Ϊ�����ڽ�ͼ�϶Գ�λ�õ�ɽ�ĸ߶Ȳ�ľ���ֵ֮�ͣ���ͼ��������ҵ�ɽ�ĸ߶Ȳ�����ڶ��������ڶ���ɽ�ĸ߶Ȳ�������ĺͣ���

Rebecca ��Ҫ֪�����ڳ���Ϊ $i$ �Ľ�ͼ��ӵ�е���С���Գ��ԡ�������� $1\leq i \leq N$��������ֵ��

```input1
7
3 1 4 1 5 9 2
```

```output1
0 2 0 5 2 10 10
```

```input2
4
1 3 5 6
```

```output2
0 1 3 7
```

## ��ʾ
Explanation of Output for Sample Input $1$:

We will show why the fifth value from the left is $2$.Let us try to compute all the asymmetric values of crops with length $5$.

The height of the mountains in the first crop is $[3, 1, 4, 1, 5]$. The asymmetric value of this crop is $|3 - 5| + |1 - 1| + |4 - 4| = 2$.

The height of the mountains in the second crop is $[1, 4, 1, 5, 9]$. The asymmetric value of this crop is $|1 - 9| + |4 - 5| + |1 - 1| = 9$.

The height of the mountains in the last crop is $[4, 1, 5, 9, 2]$. The asymmetric value of this crop is $|4 - 2| + |1 - 9| + |5 - 5| = 10$.

Hence, the most symmetric crop of length $5$ is $2$.

Explanation of Output for Sample Input $2$:

This sample satisfies the second subtask. Note that the only crop of length $4$ is $[1, 3, 5, 6]$ which has asymmetric value of $|1 - 6| + |3 - 5| = 7$.

**��������������**��

- Subtask 1��5 points����$1\leq N \leq 300$��$0\leq h_i \leq 10^5$��

- Subtask 2��5 points����$1 \leq N \leq 5000$��$0 \leq h_i \leq 10^5$����֤ɽ�ĸ߶ȴ����ҵ���������

- Subtask 3��5 points����$1\leq N\leq 5000$��$0 \leq h_i \leq 10^5$��

