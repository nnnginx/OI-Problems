## ��Ŀ����
Byteasar bought his son Bytie a set of blocks numbered from $1$ to $n$ and arranged them in a row in a certain order.

Bytie's goal is to rearrange the blocks so that they are ordered naturally, from the smallest number to the largest.

However, the only moves Bytie is allowed to make are:

putting the last block at the very beginning (move a), and                  putting the third block at the very beginning (move b).

Help Bytie by writing a program that tells whether a given arrangement of    blocks can be properly reordered, and tells the right sequence of moves if it is.


## �����ʽ
In the first line of the standard input there is a single integer $n$, $1\le n\le 2\ 000$.

In the second line there are $n$ integers from the range $1$ to $n$, separated by single spaces.

No number appears twice, and thus they represent the initial arrangement of the blocks.


## �����ʽ
If there is no sequence of moves leading to an arrangement with increasing blocks' numbers, your program should print out "NIE DA SIE" (there is no way in Polish), without the quotation marks.

Otherwise there should be a single integer $m$ ($m\le n^2$), denoting the number of operations, in the first line.

An operation is a $k$-fold execution of either a or b move.

If $m>0$, then there should be a sequence of $m$ integers with either a or b appended in the second line.

Thus $k$a (for $0<k<n$) denotes the $k$-fold execution of the move a.

Analogously, $k$b (for $0<k<n$) denotes the $k$-fold execution of the move b.

Furthermore, the characters appended to the numbers in the second line have to alternate.

Should there be more than one solution, your program is free to pick one arbitrarily.


## ��Ŀ����
### ��Ŀ����

**���� POI 2011 Round 1. D��[Shift](https://szkopul.edu.pl/problemset/problem/n6S4y9QrbGqYUz64e2O-OV7D/site/?key=statement)��**

Byteasar �����Ķ��� Bytie ����һ�й� $ n $ ���ľ��������Щ��ľ�� $ 1 $ �� $ n $ ��ţ�������һ����˳��ڳ�һ�š�Bytie Ҫ����Щ��ľ���ձ�Ŵ�С�����˳���������У�����ֻ�����������ֲ�����

* ���� a�������һ����ľ�Ƶ���ǰ�档
* ���� b���ѵ�������ľ�Ƶ���ǰ�档

���ǽ��������� $ k $ ��ͬһ��������Ϊ��һ�����������ʾΪ $ k a $ �� $ k b $��  
����Ҫ���� Bytie дһ�����򣬸�������û��һ�����������ܹ�ʹ��ľ���ձ�Ŵ�С�����˳���������У����������������С�

### �����ʽ

����ĵ�һ�а���һ������ $ n $����ʾ��ľ�ĸ�����
�ڶ��а��� $ n $ ����������ʾ��ľ��ʼ������˳��û���ظ������֡�

### �����ʽ

���û��һ�ַ����ܽ���ľ���ձ�Ŵ�С�����˳���������У���Ӧ����� `NIE DA SIE`���������е� `There is no way`����

���򣬵�һ����Ӧ�����һ������ $ m $����ʾ������**����**��$ m $ �������� $ m \le n^2 $��  
�ڶ��б�ʾ�� $ m $ �������ÿ�����֮���ÿո������  
ÿһ����������� $ k $ �Ͳ�����ʽ���м�**û��**�ո��� `3a`��$ 3 $ �� a ��������  
��Ҫ��������������������಻ͬ��ÿ������н��еĴ��� $ 0 \lt k \lt n $��

### ���ݷ�Χ

���� $ 100\% $ �����ݣ�$ 1 \le n \le 2000 $��

���������� [LibreOJ](https://loj.ac/p/2158)��checker ������ [����](https://www.luogu.com.cn/discuss/70755)��

```input1
4
1 3 2 4
```

```output1
4
3a 2b 2a 2b
```

