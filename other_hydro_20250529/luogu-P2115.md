## ��Ŀ����
Farmer John's arch-nemesis, Farmer Paul, has decided to sabotage Farmer John's milking equipment!

The milking equipment consists of a row of N (3 <= N <= 100,000) milking machines, where the ith machine produces M\_i units of milk (1 <= M\_i <= 10,000).  Farmer Paul plans to disconnect a contiguous block of these machines -- from the ith machine up to the jth machine (2 <= i <= j <= N-1); note that Farmer Paul does not want to disconnect either the first or the last machine, since this will make his plot too easy to discover.  Farmer Paul's goal is to minimize the average milk production of the remaining machines.  Farmer Paul plans to remove at least 1 cow, even if it would be better for him to avoid sabotage entirely.

Fortunately, Farmer John has learned of Farmer Paul's evil plot, and he is wondering how bad his milk production will suffer if the plot succeeds.  Please help Farmer John figure out the minimum average milk production of the remaining machines if Farmer Paul does succeed.

ũ��Լ����ͷ�ŵ��˱��޾����ƻ�ũ��Լ���ļ����豸�������豸�ų�һ�У���N��3<= N <=100000��̨���̻������е�i��̨���̻�����M\_i��λ��1 <= M\_i<=10,000����ţ�̡�


���޼ƻ��ж�һ�������ļ��̻����ӵ�į���̻�����j̨���̻���2<= i<= j<= N-1����ע�⣬����ϣ���Ͽ���һ̨�����һ̨���̻�����Ϊ�⽫��ʹ���ļƻ�̫���ױ����֡����޵�Ŀ���������������ƽ����������С�����޼ƻ���ȥ����1̨���̻���

�����ʣ���������Сƽ����������


## �����ʽ
�� 1 �У�һ������ N��

�� 2 �� N+1 �У��� i+1 �а���һ������ M\_i��


## �����ʽ
�� 1 �У� һ��ʵ���� ��ʾƽ��ţ�̲�������Сֵ�� ������λС�� ���������룩��


```input1
5
5
1
7
8
2
```

```output1
2.667
```

## ��ʾ
������˵����

��ȥ 7 �� 8��ʣ�� 5, 1, 2��ƽ��ֵΪ 8/3��

�����ݹ�ģ��Լ����

���� 30%�����ݣ�N <= 1,000��

���� 50%�����ݣ�N <= 10,000��

���� 100%�����ݣ�3 <= N <= 100,000��1 <= M\_i <= 10,000��

��ʱ�����ơ�

0.2s/128M


