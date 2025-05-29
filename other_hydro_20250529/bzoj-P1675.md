## ��Ŀ����

It's election time. The farm is partitioned into a 5x5 grid of cow locations, each of which holds either a Holstein ('H') or Jersey ('J') cow. The Jerseys want to create a voting district of 7 contiguous (vertically or horizontally) cow locationssuch that the Jerseys outnumber the Holsteins. How many ways can this be done for the supplied grid?

ũ��������Ϊ $5*5$ �ĸ��ӣ�ÿ�������ж���һͷ��ţ������ֻ�к�˹̹�����Ϊ `H` ���ͽܶ��������Ϊ `J` ������Ʒ�֡�  

���һͷ��ţ����һͷ���������ĸ������е���һ�������˵����������  

��ţҪ��ѡ�ˡ�������һֻ�ܶ�����ţ����ѡ�� $7$ ͷ��������ţ������һ����ѡ����ʹ����������Ʒ�ֵ���ţ�Ⱥ�˹̹�ĶࡣҪ�����дһ�������������������

## �����ʽ

Lines 1..5: Each of the five lines contains five characters per line, each 'H' or 'J'. No spaces are present.

5�У�����ũ���������

## �����ʽ

Line 1: The number of distinct districts of 7 connected cows such that the Jerseys outnumber the Holsteins in the district.

�����������������

```input1
HHHHH
JHJHJ
HHHHH
HJHHJ
HHHHH
```

```output1
2
```

## ���ݹ�ģ��Լ��

�ޡ�

## ��ʾ

![](./1225/file/pic1.jpg)

## ��Ŀ��Դ

[Silver](http://www.lydsy.com/JudgeOnline/problemset.php?search=Silver)
