## ��Ŀ����
Bessie has gotten herself stuck on the wrong side of Farmer John's barn again, and since her vision is so poor, she needs your help navigating across the barn.

The barn is described by an $N \times N$ grid of square cells ($2 \leq N \leq 20$), some being empty and some containing impassable haybales. Bessie starts in the lower-left corner (cell 1,1) and wants to move to the upper-right corner (cell $N,N$). You can guide her by telling her a sequence of instructions, each of which is either "forward", "turn left 90 degrees", or "turn right 90 degrees". You want to issue the shortest sequence of instructions that will guide her to her destination. If you instruct Bessie to move off the grid (i.e., into the barn wall) or into a haybale, she will not move and will skip to the next command in your sequence.

Unfortunately, Bessie doesn't know if she starts out facing up (towards cell 1,2) or right (towards cell 2,1). You need to give the shortest sequence of directions that will guide her to the goal regardless of which case is true. Once she reaches the goal she will ignore further commands.



## �����ʽ
The first line of input contains $N$.

Each of the $N$ following lines contains a string of exactly $N$ characters, representing the barn. The first character of the last line is cell 1,1. The last character of the first line is cell N, N.

Each character will either be an H to represent a haybale or an E to represent an empty square.

It is guaranteed that cells 1,1 and $N,N$ will be empty, and furthermore it is guaranteed that there is a path of empty squares from cell 1,1 to cell $N, N$.


## �����ʽ
On a single line of output, output the length of the shortest sequence of directions that will guide Bessie to the goal, irrespective whether she starts facing up or right.


## ��Ŀ����
### ��Ŀ����

Bessie ��һ�α������� Farmer John �ĹȲֵĴ���һ�࣬�������������ܲ����Ҫ��İ����������Ȳ֡�

�Ȳ���һ�� $N \times N$ �ķ�������������$2 \leq N \leq 20$��������һЩ�����ǿյģ���һЩ������޷�ͨ���ĸɲݶѡ�Bessie �����½ǣ����� 1,1����ʼ����Ҫ�ƶ������Ͻǣ����� $N,N$���������ͨ��������һϵ��ָ������������ÿ��ָ������ǡ�ǰ������������ת 90 �ȡ�������ת 90 �ȡ�������Ҫ������̵�ָ�����У�������������Ŀ�ĵء������ָʾ Bessie �ƶ��������⣨��ײ���Ȳ�ǽ�ڣ������ɲݶѣ����������ƶ����������������е���һ��ָ�

���ҵ��ǣ�Bessie ��֪����������泯�ϣ�������� 1,2�������泯�ң�������� 2,1��������Ҫ����һ����̵�ָ�����У�����������泯�ĸ����򣬶�������������Ŀ�ꡣһ��������Ŀ�꣬�������Ժ�����ָ�

### �����ʽ

����ĵ�һ�а��� $N$��

�������� $N$ ��ÿ�а���һ������Ϊ $N$ ���ַ�������ʾ�Ȳ֡����һ�еĵ�һ���ַ��Ǹ��� 1,1����һ�е����һ���ַ��Ǹ��� $N,N$��

ÿ���ַ�Ҫô�� H ��ʾ�ɲݶѣ�Ҫô�� E ��ʾ�շ���

��֤���� 1,1 �� $N,N$ �ǿյģ����ұ�֤����һ���Ӹ��� 1,1 ������ $N,N$ �Ŀշ���·����

### �����ʽ

���һ�У���ʾ���� Bessie ����泯�ĸ����򣬶�������������Ŀ������ָ�����еĳ��ȡ�

```input1
3
EHE
EEE
EEE
```

```output1
9
```

