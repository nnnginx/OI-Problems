## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/dqo3q5sa.png)

## �����ʽ
There are one or more test cases in the input. Each case starts with a line giving two integers N and M, where N is the number of rows of the map, and M is the number of columns. The rest of the input will be N lines describing the map. You may assume both N and M are between 2 and 100, inclusive. There will be the same number of 'H's and
'm's on the map; and there will be at most 100 houses. Input will terminate with 0 0 for N and M.

## �����ʽ
For each test case, output one line with the single integer, which is the minimum amount, in dollars, you need to pay. 

## ��Ŀ����
# �ؼ�

## ��Ŀ����
�������ͼ���� $n$ ���˺� $n$ �����ӡ���ÿ����λʱ���ÿ���˶����������ڵĵ���ˮƽ��ֱ�ƶ�һ����λ��������ÿ���ˣ�����ҪΪ��ÿ��һ��֧�� $1$ ��Ԫ�����зѣ�ֱ��������һ�����ӡ�����ÿ������ֻ������һ���ˣ���������ܸ��ӡ�  
��������Ǽ�������Ҫ֧������ͽ��Ա㽫�� $n$ �����͵��� $n$ ����ͬ�ķ���������ǳ����ĵ�ͼ��`.` ��ʾ�հ׿ռ䣬`H`��ʾ�õ��ϵķ��ӣ�`m`��ʾ�ڸõ�����һ���ˡ�  
����԰������ͼ�ϵ�ÿ���������һ���൱��������Σ�����������ͬʱ���� $n$ ��������⣬���һ������û�н��뷿�ӵ�����²����з��ӵ������ϣ�Ҳû��ϵ��

## �����ʽ

��������һ����������������ÿ���������һ�и����������� $N$ �� $M$ ��ʼ������ $N$ ��ӳ���������$M$ ����������������뽫��������ͼ�� $N$ �С�����Լ��� $N$ �� $M$ ���� $2$ �� $100$ ֮�䣬���� $2$ �� $100$��������ͬ������ $H$ �� $m$ �ڵ�ͼ�ϣ������ $100$ �����ӡ�$N$ �� $M$ �����뽫��`0 0`��ֹ��

## �����ʽ

����ÿ���������������һ�д��е��������Ĵ��룬��������Ҫ֧������С����Ԫ����

---
�����ṩ�ߣ�[csyc5586](https://www.luogu.com/user/668156)

```input1
2 2
.m
H.
5 5 
HH..m 
..... 
.....
.....
mm..H
7 8
...H....
...H....
...H.... 
mmmHmmmm 
...H.... 
...H.... 
...H.... 
0 0
```

```output1
2
10
28
```

