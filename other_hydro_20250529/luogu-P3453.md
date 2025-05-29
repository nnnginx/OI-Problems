## ��Ŀ����
Byteasar has a cottage. Lately, he has bought $n$ trees and had them planted all in one row. Byteasar does not,  however, like the order which the trees have been planted in. It particularly annoys him that tall and short  ones have been mixed up, and the composition does not meet his aesthetic criteria.

Byteasar has invented a disorder coefficient so as to allow the gardener to comprehend his intentions: thelower the value of the coefficient the prettier the row of trees. It is defined in the following way:

$|h_1-h_2|+|h_2-h_3|+\cdots+|h_{n-1}-h_n|$, where $h_1,h_2,\cdots,h_n$ are the heights of consecutive trees in a row.
Replanting is a very toilsome and cumbersome task, therefore Byteasar has ordered the gardener to replanttwo trees at the most (i.e. interchange their positions). The task of the gardener is to choose the pair to replantin a way that makes the disorder coefficient the smallest.

The gardener is not sure if he has chosen the correct pair of trees and he fears he may lose his job ifhe is mistaken. Help him: for each tree calculate the minimal disorder coefficient that may be attained byswitching places with any other tree.

TaskWrite a programme which:

reads the height of the consecutive trees in a row from the standard input,        for each tree calculates the minimal disorder coefficient that may be attained should it switch places    with some other tree (or should there be no change at all),        writes the outcome to the standard output.

����һ�����Ĳ�����̶�Ϊ���������ĸ߶Ȳ�ĺ͡������߷ֱ�Ϊ $h _ 1, h _ 2, \cdots, h _ n$����ô������̶ȶ���Ϊ��$|h_1-h_2|+|h_2-h_3|+\cdots+|h_{n-1}-h_n|$��

�����ÿ�� $i$ ��������ֻ�� $i$ ����һ���������߶ȣ����Բ�����������ô���������С�Ƕ��١�


## �����ʽ
The first line of the standard input contains one integer $n$ ($2\le n\le 50\ 000$).

The other contains $n$ integers $h_i$ ($1\le h_i\le 100\ 000\ 000$)separated by single spaces, denoting the height of the consecutive trees in the row.


## �����ʽ
The output should consist of precisely $n$ lines. The $i$'th line should contain a single integer - the smallestdisorder coefficient attainable when considering replanting of the $i$'th tree.


```input1
5
7 4 5 2 5
```

```output1
7
7
8
7
7
```

