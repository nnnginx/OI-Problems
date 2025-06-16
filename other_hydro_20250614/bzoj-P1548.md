## ��Ŀ����
A group of $n$ children are playing with a set of $n^2$ flat square blocks. Each block is painted from above with one colour, and there are no more than $2$ blocks of each colour. The blocks are initially arranged in an $n^2$ square forming some sort of picture.

The children have been provided with some other $n^2$ picture and asked to rearrange the blocks to that form. Since this is not really what they enjoy doing most, they intend to solve the task together and spend as little time on it as possible. Thus, every minute each child chooses a single $1 \times n$ row or $n \times 1$ column of blocks to rearrange. This row/column may never intersect with rows/columns chosen by other children in the same minute. A child takes one minute to perform any rearrangement (permutation) of the blocks within its row/column it likes.

Determine whether the children can perform their task of converting one block image into the other, and if so -- find the minimum possible time in minutes required to achieve this.

![](https://hydro.org.cn/d/bzoj/p/1548/file/pic1%20(8).jpg)

һȺ $n$ ����������һ�� $n^2$ ����ƽ���顣ÿ���鶼����һ����ɫ���Ƶģ�ÿ����ɫ���ֻ�ܴ����� $2$ �����ϡ���Щ������������γ�ĳ��ͼƬ�� $n^2$ �������С�

���ڸ��������ṩ��һ����СΪ $n^2$ ͼƬ����Ҫ�������������иñ�����ʽ�������Ⲣ����������ϲ���������飬��ˣ����Ǵ��㹲ͬ������񣬲������ٵ�ʱ���������ϡ���ˣ�ÿ������ÿ���Ӷ���ѡ��һ�л�һ�����������С�����/�п�����Զ������ͬһʱ����������ѡ�����/���ཻ��������Ҫһ���ӵ�ʱ�����ϲ������/���еĿ�����κ��������С�

ȷ���������Ƿ����ִ�н�һ����ͼ��ת��Ϊ��һ����ͼ�������������ԣ����ҵ��ﵽ��Ŀ����������ʱ�䣨�Է���Ϊ��λ���� 

Translated by wheneveright.

## �����ʽ
��һ��һ���� $t$����ʾ�������ݵ�������

ÿһ���һ��һ���� $n$����ʾ���̵Ĵ�С��

������ $n$ �У�ÿ�� $n$ �������� $i$ �е� $j$ ��һ���� $a_{i,j}$ ��ʾ��ʼ�����е�ÿһ�������ٽ����� $n$ �У�ÿ�� $n$ �������� $i$ �е� $j$ ��һ���� $b_{i,j}$ ��ʾĿ�������е�ÿһ������

## �����ʽ
����ÿ�����ݣ��㶼Ҫ���һ����С�ı任����������ʼ״̬���ܱ任��Ŀ��״̬����� `no`��

## ��������
```plain
10
3
5 5 6 
3 2 4 
7 2 1 
2 4 2 
5 1 6 
5 7 3 
3
3 3 5 
6 2 1 
1 6 9 
3 1 3 
5 6 1 
2 6 9 
3
7 8 3 
8 5 5 
3 4 1 
1 7 3 
8 8 4 
5 5 3 
3
4 2 6 
8 1 4 
8 1 3 
2 3 4 
4 6 8 
1 1 8 
3
2 7 1 
3 2 5 
8 8 9 
5 8 8 
1 9 2 
2 7 3 
3
7 8 3 
3 6 2 
2 1 6 
2 6 8 
1 2 6 
7 3 3 
3
2 8 3 
7 2 8 
6 5 4 
8 7 6 
5 2 4 
2 3 8 
3
1 6 8 
9 8 1 
3 3 5 
8 1 9 
8 6 1 
3 3 5 
3
7 9 4 
9 7 1 
2 2 4 
2 7 4 
1 9 4 
7 9 2 
3
6 2 2 
8 6 1 
7 3 5 
2 6 6 
7 2 3 
1 8 5 

```
## �������
```plain
3
2
3
2
3
2
3
2
3
3
```

## ���ݹ�ģ��Լ��

| ���Ե� | t | n | ʱ�� |
| ----------- | ----------- | ----------- | ----------- |
| 1 | t=10 | n=3 | 1s |
| 2 | t=10 | n<=10 | 1s |
| 3 | t=50 | n<=10 | 1s |
| 4-5 | t=200 | n<=100 | 2s |
| 6-7 | t=200 | n<=200 | 7s |
| 8-10 | t=200 | n=200 | 15s |

�����������ݱ�֤ $a_{i,j},b_{i,j}\le n^2$��

## ��Ŀ��Դ
HNOI2009 ��ѵ Day4