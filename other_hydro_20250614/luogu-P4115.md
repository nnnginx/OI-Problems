## ��Ŀ����
#��ӭ�ṩ��ǿ�����ݣ�����Ŀ֧�����޼����ݣ���˽�ţ��ٶ����̵�ַ��

#���ݷ�Χ��spoj���в�ͬ


## ��Ŀ����
����һ�ñߴ�Ȩ�Ľڵ�����Ϊn��������ʼ�������нڵ㶼�ǰ�ɫ�������ֲ�����

C x���ı�ڵ�x����ɫ�����ױ�ڣ��ڱ��

A��ѯ��������Զ��������ɫ�ڵ�ľ��룬��������ɫ�ڵ�����غ�(��ʱ����Ϊ0)��


## �����ʽ
In the first line there is an integer N (N <= 100000)

In the next N-1 lines, the i-th line describes the i-th edge: a line with three integers a b c denotes an edge between a, b of value c (-1000 <= c <= 1000)

In the next line, there is an integer Q denotes the number of instructions (Q <= 200000)

In the next Q lines, each line contains an instruction "C a" or "A"


## �����ʽ
For each "A" operation, write one integer representing its result. If there is no white node in the tree, you should write "They have disappeared.".


```input1
3
1 2 1
1 3 1
7
A
C 1
A
C 2
A
C 3
A
```

```output1
2
2
0
They have disappeared.
```

