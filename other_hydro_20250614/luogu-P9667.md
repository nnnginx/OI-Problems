## ��Ŀ����
Prof. Pang built $n$ block towers with different heights. The $i$-th tower has height $a_i$.

Prof. Shou doesn't like these towers because of their arbitrary heights. He decides to $\textbf{first remove exactly \textit{m} of them}$, and then perform some (or none) of the following operations: 

- Choose a tower and increase its height $a_i$ by $1$. 
- Choose a tower and decrease its height $a_i$ by $1$.
- Choose a tower and divide its height $a_i$ by $2$. If the new height is not an integer, it is rounded down. 

Prof. Shou can never choose a removed tower. If after an operation, the height of a tower will become $0$, that operation is not allowed. Under these constraints, Prof. Shou can perform an arbitrary number of operations in arbitrary order. 

Prof. Shou would like all the towers that are not removed to have the same heights. Please calculate the minimum number of operations to achieve this.

## �����ʽ
The first line contains one integer $T~(1\le T \le 10)$, the number of test cases.

For each test case, the first line contains two integers $n, m~(1\le n\le 500, 0\le m <n)$, the number of towers, and the number of towers Prof. Shou should delete before performing the operations.

The next line contains $n$ integers $a_1,\ldots, a_n~(1\le a_i\le 10^9)$, the initial heights of the towers.

## �����ʽ
For each test case, output the minimum number of operations in one line.

## ��Ŀ����
### ��Ŀ����
�ӽ��ڴ��� $n$ ����ͬ�߶ȵ������� $i$ �����ĸ߶��� $a _ {i}$��

�ٽ��ڲ�ϲ����Щ�β�������������**��ȥ�������е� $m$ ��**��Ȼ��ִ�����²����е�һЩ����ִ�У���
- ѡ��һ������������ $1$ ����λ�߶ȡ�
- ѡ��һ������������ $1$ ����λ�߶ȡ�
- ѡ��һ�����������ĸ߶� $a _ {i}$ ���� $2$����������������Ļ�������ȡ����

�ٽ�����Զ����ѡ�񱻲��������������������ĸ߶ȱ�Ϊ $0$�����������������ЩԼ�������£��ٽ��ڿ��԰�����˳��ִ���������������㡣

�ٽ���ϣ������û�б��������������ͬ�ĸ߶� $a _ {i}$�������ʵ�ִ�Ŀ�����С����������
### �����ʽ
��һ����һ������ $T(1\leqslant$ $T$ $\leqslant$ $10)$,��ʾ�� $T$ �����ݡ�

����ÿ��������ݣ���һ�а����������� $n,m (1\leqslant$ $n$ $\leqslant$ $500$$,$$0$ $\leqslant$ $m$ $\leqslant$ $n$$)$����ʾ���������Լ��ٽ�����ִ�в���֮ǰӦ��ɾ��������������

��һ�а��� $n$ ������ $a _ {1},\dots,a _ {n} (1\leqslant$ $a _ {i}$ $\leqslant$ $10^9)$����ʾ��������߶ȡ�
### �����ʽ
����ÿ��������ݣ���һ���������С��������

```input1
3
2 0
2 6
5 0
1 2 3 4 5
5 3
1 2 3 4 5
```

```output1
2
4
1
```

