## ��Ŀ����
A book is being typeset using a fixed width font and a simple greedy algorithm to fill each line. The
book contents is just a sequence of words, where each word contains one or more characters.

## ��Ŀ����
Before typesetting, we choose a maximum line length and denote this value with m. Each line can be at most m characters long including the space characters between the words. The typesetting algorithm simply processes words one by one and prints each word with exactly one space character between two consecutive words on the same line. If printing the word on the current line would exceed the maximum line length m, a new line is started instead.

![](https://cdn.luogu.com.cn/upload/pic/16228.png)

You are given a text to be typeset and are experimenting with different values of the maximum line length m. For a fixed m, the leading sentence is a sentence (a sequence of words separated with a single space character) formed by the first words of lines top to bottom. In the example above, when the sample text is typeset with the maximum line length 14, the leading sentence is ��its to you n��.

Given a text and two integers a and b, find the length of the leading sentence for every candidate maximum line length between a and b inclusive. The length of a sentence is the total number of characters it contains including the space characters.

## �����ʽ
The first line contains the text to be typeset �C a sequence of words separated by exactly one space character. Each word is a string consisting of one or more lowercase letters from the English alphabet.

The second line contains two integers a and b �C the edges of the interval we are interested in, as described above.

It is guaranteed that $1<=w<=a<=b<=z<=500 000$, where w is the length of the longest word in the text and z is the total number of characters in the text including the space characters.

## �����ʽ
Output $b - a + 1$ lines �C the $k$-th of those lines should contain a single integer �C the total length of the leading sentence when the maximum line length is equal to $a - 1 + k$.

## ��Ŀ����

����һ����,�ù̶���ȵ�����ͼ򵥵�̰���㷨�����ÿ�����֡����������һ���������У�ÿ�����ʰ���һ�������ַ���

�Ű�ǰ������ѡ��һ�������г��ȣ�����m��ʾ���ֵ��ÿ����������m���ַ�����������֮��Ŀո��ַ�����ʹ���Ű��㷨�򵥵���������ʣ�����ͬһ���ϵ�������������֮���ӡÿ�����ʣ�ÿ������ֻ��һ���ո��ַ�����������ڵ�ǰ���ϴ�ӡ���ֳ�������г���m����ʼ���С�
![](https://cdn.luogu.org/upload/pic/16228.png)
������õ���һ��Ҫ�Ű���ı�������������������г���m�Ĳ�ֵͬ�����ڹ̶�m��ǰ������һ������(��һ���ո��ַ��ָ���һϵ�е���)�����еĵ�һ�����ʴ��ϵ�����ɡ��������У��������ı�������г���14�����Ű�ʱ��ǰ�����ǡ�������˵��n����its to you n��
����һ���ı�����������a��b���ҳ�a��b֮��ÿ����ѡ����г��ȵ�ǰ���䳤�ȡ����ӵĳ��������������ַ������������ո��ַ�

**�����ʽ��**
��һ�а���Ҫ�Ű���ı�������һ���ո��ַ��ָ���һϵ�е��ʡ�ÿ�����ʶ���һ���ַ�������Ӣ����ĸ���е�һ������Сд��ĸ��ɡ� �ڶ��а�����������a��b�������������������Ե����֤1<=w <=a<=b<=z<=50000,
����w���ı�������ʵĳ��ȣ�z���ı��а����ո��ַ����ַ�������

**�����ʽ**
���b-a+1�С�����Щ�еĵ�k��Ӧ�ð���һ��������������г��ȵ���a-1+kʱǰ������ܳ��ȡ�

**�����������**

��������#1
```
its a long way to the top if you wanna rock n roll
13 16
```
�������#1
```
22
12
12
15
```

```input1
its a long way to the top if you wanna rock n roll
13 16
```

```output1
22
12
12
15
```

## ��ʾ
Central Europe Regional Contest 2015
Problem B

