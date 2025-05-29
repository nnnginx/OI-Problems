## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/tsc2hi05.png)

## ��Ŀ����
Matryoshkas are sets of traditional Russian wooden dolls of decreasing size placed one inside the other. A matryoshka doll can be opened to reveal a smaller figure of the same sort inside, which has, in turn, another figure inside, and so on.

The Russian Matryoshka Museum recently exhibited a collection of similarly designed matryoshka sets, differing only in the number of nested dolls in each set. Unfortunately, some over-zealous (and obviously unsupervised) children separated these sets, placing all the individual dolls in a row. There are $n$ dolls in the row, each with an integer size. You need to reassemble the matryoshka sets, knowing neither the number of sets nor the number of dolls in each set. You know only that every complete set consists of dolls with consecutive sizes from $1$ to some number $m$, which may vary between the different sets.

When reassembling the sets, you must follow these rules:
- You can put a doll or a nested group of dolls only inside a larger doll.
- You can combine two groups of dolls only if they are adjacent in the row.
- Once a doll becomes a member of a group, it cannot be transferred to another group or permanently separated from the group. It can be temporarily separated only when combining two groups.

Your time is valuable, and you want to do this reassembly process as quickly as possible. The only time-consuming part of this task is opening and subsequently closing a doll, so you want to minimize how often you do this. For example, the minimum number of openings (and subsequent closings) when combining group $[1, 2, 6]$ with the group $[4]$ is two, since you have to open the dolls with sizes $6$ and $4$. When combining group $[1, 2, 5]$ with the group $[3, 4]$, you need to perform three openings.

Write a program to calculate the minimum number of openings required to combine all disassembled matryoshka sets.

## �����ʽ
The input consists of a single test case. A test case consists of two lines. The first line contains one integer $n (1 \leq n \leq 500)$ representing the number of individual dolls in the row. The second line contains $n$ positive integers specifying the sizes of the dolls in the order they appear in the row. Each size is between $1$ and $500$ inclusive.

## �����ʽ
Display the minimum number of openings required when reassembling the matryoshka sets. If reassembling cannot be done (some of the kids might have been excessively zealous and taken some dolls), display the word `Impossible`.

## ��Ŀ����
**����Ŀ������**

�����Ƕ���˹��ͳľ����ߣ���һ���𽥱�С��������ɣ����η�������һ�������ڲ���һ�����޿��Դ򿪣�¶��һ����С��������ż���������ż�ڲ�������һ����ż���Դ����ơ�

����˹���޲�������չ����һϵ��������Ƶ����ޣ���֮ͬ��������ÿ��������Ƕ�׵�������ͬ�����ҵ��ǣ�һЩ�������ģ���Ȼû�еõ��ල���ĺ��Ӱ���Щ���޲�ɢ�ˣ��������еĵ��������ų�һ�С�������һ������ $n$ �����ޣ�ÿ������һ��������С������Ҫ������װ��Щ���ޣ��Ȳ�֪�����޵�������Ҳ��֪��ÿ�����������޵���������ֻ֪��ÿ�������������ɴ�С�� $1$ ��ĳ������ $m$ ��������С��������ɣ���������� $m$ �ڲ�ͬ�������п���������ͬ��

��������װ����ʱ���������ѭ���¹���
- ��ֻ�ܽ�һ�����޻�һ��Ƕ�׵����������һ������������С�
- ��ֻ�ܺϲ��������������ڵ������顣
- һ��һ�����޳�Ϊһ����ĳ�Ա�������ܱ�ת�Ƶ���һ��������õش����з��롣��ֻ���ںϲ�������ʱ��ʱ���롣

���ʱ��ǳ�������ϣ������������������װ���̡����������Ψһ��ʱ�Ĳ����Ǵ򿪺����ر�һ�����ޣ������ϣ���������������Ĳ������������磬������ $[1, 2, 6]$ ���� $[4]$ �ϲ�ʱ��������Ҫ�������ο��ز�������Ϊ�����򿪴�СΪ $6$ �� $4$ �����ޡ��������� $[1, 2, 5]$ ���� $[3, 4]$ �ϲ�ʱ����Ҫ�������ο��ز�����

��дһ���������������װ���в�ɢ��������������ٿ��ش�����

**�������ʽ��**

�������һ����������������������������ɡ���һ�а���һ������ $n (1 \leq n \leq 500)$����ʾ���е������޵��������ڶ��а��� $n$ �����������������������г��ֵ�˳��ָ�����޵Ĵ�С��ÿ����С�� $1$ �� $500$ ֮�䣨���� $1$ �� $500$����

**�������ʽ��**

���������װ������������ٿ��ش��������������װ�޷���ɣ�������Щ���ӹ������ģ�������һЩ���ޣ�������� `Impossible`��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
7
1 2 1 2 4 3 3
```

```output1
Impossible
```

```input2
7
1 2 3 2 4 1 3

```

```output2
7
```

