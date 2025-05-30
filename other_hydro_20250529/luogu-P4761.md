## 题目描述
According to a popular belief, computer programmers drink a lot of coffee and know only a few words. The vocabulary of a typical programmer consists of just three words. Besides, he rarely knows how to spell them. To help programmers with their spelling mistakes, we published a book titled $The \ Dictionary \ of \ the \ Three \ Words \ Every \ Typical \ Programmer \ Should \ Know$.

You got a copy of the book but, soon after that, you spilled your coffee over it.

Now, youcannot read some of the characters. Fortunately, the three words were, as usually in dictionaries,distinct and printed in lexicographical order.
Before you attempt to use that fact to recover the missing characters, you want to know in how many different ways you can do it. Since you expect this number might be large, you want to know it modulo $10^9 + 9$.

## 输入格式
The first line of input contains the number of test cases $T$. The descriptions of the test cases follow:

Each test case consists of three lines, each containing a single nonempty word – in the order they appear in the dictionary. Words consist of small letters of the English alphabet and question marks, the latter denoting missing characters. Each word is at most $1 000 000$ characters long.


## 输出格式
For each test case, output one line containing the number of different ways you can substitute each question mark with one of the $26$ letters from ``a`` to ``z`` in such a way that the three words are distinct and in lexicographical order. The number should be printed modulo $10^9 + 9$.

## 题目大意
给你三个字符串，这些字符串有些单词模糊不可认了，用"?"来代表。
现在你可以用任意英文小写字母来代表它们。要求是使得给定的三个字符串中
所有的"?"被你认定的字母代替后，各不相同且按字典序出现。问有多少种方式。

输入：先给出一个数字N，代表数据组数。
接下来3*N行，每行给出一个字符串。长度<=1000 000

输出：输出结果 Mod 10^9+9

```input1
3
?heoret?cal
c?mputer
?cience
jagiellonian
?niversity
kra?ow
?
b
c
```

```output1
42562
52
1
```

