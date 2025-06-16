## ��Ŀ����
In the Byteotian Training Centre, the pilots prepare for missions requiring extraordinary precision and control.

One measure of a pilot's capability is the duration he is able to fly along a desired route without deviating too much -    simply put, whether he can fly steadily. This is not an easy task, as the simulator is so sensitive that it registers    even a slightest move of the yoke1.

At each moment the simulator stores a single parameter describing the yoke's position.

Before each training session a certain tolerance level ![](http://main.edu.pl/images/OI17/pil-en-tex.1.png) is set.

The pilots' task then is to fly as long as they can in such a way that all the yoke's position measured during the    flight differ by at most ![](http://main.edu.pl/images/OI17/pil-en-tex.2.png). In other words, a fragment of the flight starting at time ![](http://main.edu.pl/images/OI17/pil-en-tex.3.png) and ending at time ![](http://main.edu.pl/images/OI17/pil-en-tex.4.png)    is within tolerance level ![](http://main.edu.pl/images/OI17/pil-en-tex.5.png) if the position measurements, starting with ![](http://main.edu.pl/images/OI17/pil-en-tex.6.png)-th and ending with ![](http://main.edu.pl/images/OI17/pil-en-tex.7.png)-th,    form such a sequence ![](http://main.edu.pl/images/OI17/pil-en-tex.8.png) that for all elements ![](http://main.edu.pl/images/OI17/pil-en-tex.9.png) of this sequence, the inequality ![](http://main.edu.pl/images/OI17/pil-en-tex.10.png) holds.

Your task is to write a program that, given a number ![](http://main.edu.pl/images/OI17/pil-en-tex.11.png) and the sequence of yoke's position measurements,    determines the length of the longest fragment of the flight that is within the tolerance level ![](http://main.edu.pl/images/OI17/pil-en-tex.12.png).

���� $n, k$ ��һ������Ϊ $n$ �����У���������ֵ��Сֵ������ $k$ ���ӶΡ�

## �����ʽ
In the first line of the standard input two integers are given, ![](http://main.edu.pl/images/OI17/pil-en-tex.13.png) and ![](http://main.edu.pl/images/OI17/pil-en-tex.14.png)      (![](http://main.edu.pl/images/OI17/pil-en-tex.15.png), ![](http://main.edu.pl/images/OI17/pil-en-tex.16.png)), separated by a single space,      denoting the tolerance level and the number of yoke's position measurements taken.

The second line gives those measurements, separated by single spaces. Each measurement      is an integer from the interval from ![](http://main.edu.pl/images/OI17/pil-en-tex.17.png) to ![](http://main.edu.pl/images/OI17/pil-en-tex.18.png).

��һ�������ɿո���������� $k, n$��$0\leq k\leq 2\times 10 ^ 9$��$1\leq n\leq 3\times 10 ^ 6$����$k$ ��ʾ�趨�ļ�������ֵ��$n$ ��ʾ���еĳ��ȡ�

�ڶ��� $n$ ���ɿո���������� $a_i$��$1\leq a_i\leq 2\times 10^ 9$����ʾ���С�


## �����ʽ
Your program should print a single integer to the standard output:

the maximum length of a fragment of the flight that is within the given tolerance level.

һ��������ʾ�����������Ӷεĳ������ֵ��


```input1
3 9
5 1 3 5 8 6 6 9 10
```

```output1
4
```

## ��ʾ
�������ͣ�$5, 8, 6, 6$ �� $8, 6, 6, 9$ ����������������Ϊ $4$ ���ӶΡ�

