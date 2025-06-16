## ��Ŀ����
We consider strings consisting of lowercase letters of the English alphabet in this problem.

An initial fragment of a given string is called its prefix.

A final (terminal) fragment of a given string is called its suffix.

In particular, the empty string is both a prefix and a suffix of any string.

Two strings are cyclically equivalent if one of them can be obtained from another by    moving its certain suffix from the end of the string to its beginning.

For example, the strings ![](http://main.edu.pl/images/OI19/pre-en-tex.1.png) and ![](http://main.edu.pl/images/OI19/pre-en-tex.2.png) are cyclically equivalent, whereas the strings ![](http://main.edu.pl/images/OI19/pre-en-tex.3.png) and ![](http://main.edu.pl/images/OI19/pre-en-tex.4.png) are not.

In particular, every string is cyclically equivalent to itself.

A string ![](http://main.edu.pl/images/OI19/pre-en-tex.5.png) consisting of ![](http://main.edu.pl/images/OI19/pre-en-tex.6.png) letters is given.

We are looking for its prefix ![](http://main.edu.pl/images/OI19/pre-en-tex.7.png) and suffix ![](http://main.edu.pl/images/OI19/pre-en-tex.8.png) of equal length such that:

![](http://main.edu.pl/images/OI19/pre-en-tex.9.png) and ![](http://main.edu.pl/images/OI19/pre-en-tex.10.png) are cyclically equivalent,                  the common length of ![](http://main.edu.pl/images/OI19/pre-en-tex.11.png) and ![](http://main.edu.pl/images/OI19/pre-en-tex.12.png) does not exceed ![](http://main.edu.pl/images/OI19/pre-en-tex.13.png)        (i.e., the prefix ![](http://main.edu.pl/images/OI19/pre-en-tex.14.png) and the suffix ![](http://main.edu.pl/images/OI19/pre-en-tex.15.png) do not overlap in ![](http://main.edu.pl/images/OI19/pre-en-tex.16.png)), and                  the common length of ![](http://main.edu.pl/images/OI19/pre-en-tex.17.png) and ![](http://main.edu.pl/images/OI19/pre-en-tex.18.png) is maximized.

���������� $S_1, S_2$������ܹ��� $S_1$ ��һ����׺�ƶ�����ͷ���� $S_2$���ͳ� $S_1$ �� $S_2$ ѭ����ͬ�����紮 ababba �ʹ� abbaab ��ѭ����ͬ�ġ�

����һ������Ϊ $n$ �Ĵ� $S$���������������������� $L(L\leq \frac n 2)$��$S$ �� $L$ ǰ׺�� $S$ �� $L$ ��׺��ѭ����ͬ�ġ�

## �����ʽ
The first line of the standard input contains a single integer ![](http://main.edu.pl/images/OI19/pre-en-tex.19.png)      (![](http://main.edu.pl/images/OI19/pre-en-tex.20.png)) denoting the length of the string ![](http://main.edu.pl/images/OI19/pre-en-tex.21.png).

The second line of input contains the string ![](http://main.edu.pl/images/OI19/pre-en-tex.22.png) itself, consisting of ![](http://main.edu.pl/images/OI19/pre-en-tex.23.png) lowercase letters of the English alphabet.

In tests worth 30% of the points the condition ![](http://main.edu.pl/images/OI19/pre-en-tex.24.png) holds in addition.

In tests worth 50% of the points the condition ![](http://main.edu.pl/images/OI19/pre-en-tex.25.png) holds in addition.


## �����ʽ
Your program should print a single integer in the first and only line of the standard output,      namely the common length of the prefix ![](http://main.edu.pl/images/OI19/pre-en-tex.26.png) and the suffix ![](http://main.edu.pl/images/OI19/pre-en-tex.27.png) that we are looking for.


```input1
15
ababbabababbaab
```

```output1
6
```

## ��ʾ
���ݷ�Χ��

- ���� $30\%$ �����ݣ���֤ $n\le 500$��
- ���� $50\%$ �����ݣ���֤ $n\le 5000$��
- ���� $100\%$ ���ݣ���֤ $1\le n\le 10^6$��

