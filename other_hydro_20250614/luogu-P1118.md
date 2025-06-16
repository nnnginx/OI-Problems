## ��Ŀ����
`FJ` and his cows enjoy playing a mental game. They write down the numbers from $1$ to$ N(1 \le N  \le 10)$ in a certain order and then sum adjacent numbers to produce a new list with one fewer number.  They repeat this until only a single number is left.  For example, one instance of the game (when $N=4$) might go like this:

```cpp
    3   1   2   4
      4   3   6
        7   9
         16
```
Behind `FJ`'s back, the cows have started playing a more difficult game, in which they try to determine the starting sequence from only the final total and the number $N$.  Unfortunately, the game is a bit above `FJ`'s mental arithmetic capabilities.


Write a program to help `FJ` play the game and keep up with the cows.



## �����ʽ
��һ������������ $n,sum$��


## �����ʽ
�������һ�У�Ϊ�ֵ�����С���Ǹ��𰸡�

���޽��ʱ����ʲôҲ�������


## ��Ŀ����

����ôһ����Ϸ��

д��һ�� $1\sim n$ ������ $a$��Ȼ��ÿ�ν�������������ӣ������µ����У��ٶ������н��������Ĳ�������Ȼÿ�ι��ɵ����ж�����һ�ε����г����� $1$��ֱ��ֻʣ��һ������λ�á�

������һ�����ӣ�

- $3,1,2,4$��
- $4,3,6$��
- $7,9$��
- $16$��

���õ� $16$ ����һ�����֡�

������Ҫ����������һ����Ϸ�����֪�� $n$���Լ����õ������ֵĴ�С $sum$���������������� $a_i$��Ӧ����һ�� $1\sim n$ �����У��������ж��ֿ��ܣ�������ֵ�����С����һ����

���ǳ����� $a=\lang a_1,a_2,\cdots,a_n\rang$ ���ֵ���С������ $b=\lang b_1,b_2,\cdots,b_n\rang$ ���ֵ��򣬵��ҽ�������һ��λ�� $p$������ $a_1=b_1,a_2=b_2,\cdots,a_{p-1}=b_{p-1},a_p<b_p$��

```input1
4 16
```

```output1
3 1 2 4
```

## ��ʾ
- ���� $40\%$ �����ݣ�$1\le n\le 7$��  
- ���� $80\%$ �����ݣ�$1\le n \le 10$��
- ���� $100\%$ �����ݣ�$1\le n \le 12$��$1\le sum\le 12345$��


