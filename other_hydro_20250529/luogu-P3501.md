## 题目描述
Byteasar studies certain strings of zeroes and ones.

Let ![](http://main.edu.pl/images/OI17/ant-en-tex.1.png) be such a string. By ![](http://main.edu.pl/images/OI17/ant-en-tex.2.png) we will denote the reversed (i.e., "read backwards") string ![](http://main.edu.pl/images/OI17/ant-en-tex.3.png),    and by ![](http://main.edu.pl/images/OI17/ant-en-tex.4.png) we will denote the string obtained from ![](http://main.edu.pl/images/OI17/ant-en-tex.5.png) by changing all the zeroes to ones and ones to zeroes.

Byteasar is interested in antisymmetry, while all things symmetric bore him.

Antisymmetry however is not a mere lack of symmetry.

We will say that a (nonempty) string ![](http://main.edu.pl/images/OI17/ant-en-tex.6.png) is antisymmetric if, for every position ![](http://main.edu.pl/images/OI17/ant-en-tex.7.png) in ![](http://main.edu.pl/images/OI17/ant-en-tex.8.png),    the ![](http://main.edu.pl/images/OI17/ant-en-tex.9.png)-th last character is different than the ![](http://main.edu.pl/images/OI17/ant-en-tex.10.png)-th (first) character.

In particular, a string ![](http://main.edu.pl/images/OI17/ant-en-tex.11.png) consisting of zeroes and ones is antisymmetric if and only if    ![](http://main.edu.pl/images/OI17/ant-en-tex.12.png).

For example, the strings 00001111 and 010101 are antisymmetric, while 1001 is not.

In a given string consisting of zeroes and ones we would like to determine the number of contiguous    nonempty antisymmetric fragments.

Different fragments corresponding to the same substrings should be counted multiple times.

## 输入格式
The first line of the standard input contains an integer ![](http://main.edu.pl/images/OI17/ant-en-tex.13.png) (![](http://main.edu.pl/images/OI17/ant-en-tex.14.png)) that denotes the length of the string.

The second line gives a string of 0 and/or 1 of length ![](http://main.edu.pl/images/OI17/ant-en-tex.15.png).

There are no spaces in the string.


## 输出格式
The first and only line of the standard output should contain a single integer,      namely the number of contiguous (non empty) fragments of the given string      that are antisymmetric.


## 题目大意
### 题目描述

**译自 POI 2010 Stage 2. Day 0「[Antisymmetry](https://szkopul.edu.pl/problemset/problem/EDxOyJiFZWb_PYVaYhhnhU0-/site/?key=statement)」**

对于一个 $0/1$ 字符串，如果将这个字符串 $0$ 和 $1$ 取反后，再将整个串反过来和原串一样，就称作「反对称」字符串。比如 $00001111$ 和 $010101$ 就是反对称的，而 $1001$ 就不是。  
现在给出一个长度为 $n$ 的 $0/1$ 字符串，求它有多少个子串是反对称的，注意这里相同的子串出现在不同的位置会被重复计算。

### 输入格式

第一行一个正整数 $n$ 。  
第二行一个长度为 $n$ 的 $0/1$ 字符串。

### 输出格式

一行一个整数，表示原串的反对称子串个数。

### 提示/说明

样例的 $7$ 个反对称子串分别是：$01$（出现两次），$10$（出现两次），$0101$，$1100$ 和 $001011$。

对于 $100\%$ 的数据， $1\le n\le 500\ 000$ 。

翻译来自于 [LibreOJ](https://loj.ac/p/2452)。

```input1
8
11001011
```

```output1
7
```

