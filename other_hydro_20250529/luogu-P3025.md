## 题目描述
As has happened to so many of us, Bessie has forgotten her cowtube password. She does, however, remember some handy bits of information about it.

First, she remembers that her password (denoted as variable P) has length L (1 <= L <= 1,000) roman characters and can be split into one or more words (not necessarily unique) from a dictionary composed of NW (1 <= NW <= 1,000) unique words.  A word W\_i is defined as a sequence of 1..20 lowercase letters of the Roman alphabet ('a'..'z').

She also remembers certain letters from her password along with their positions.

Consider the following example. Bessie knows that her password looks like 'a??l?ban???????' ('?' represents a letter she cannot remember), and her dictionary has the following words:

apple
cow
farmer
banana
bananas

pies
The two possible passwords for Bessie to have are 'applebananapies' and 'applebananascow'.

Given the dictionary, and the letters that Bessie remembers, please find her password. If more than one password is valid, find the lexicographically least string that works.

就像在我们身上发生很多次的情况一样，Bessie又一次忘记了她的牛场管理员密码，她只能记得密码的一部分。


首先，她记得她的密码是长度为L（1<=L<=1000）的字符串，并且她的密码中出现过的所有单词都记录在她有NW个单词的字典中，字典中的单词Wi是由1-20个字母组成的单词。


她只记得她的密码中的一部分字母和它的位置。例如，Bessie记得她的密码为“a??l?ban???????”（其中，？是她不能记得的字母），她的字典中有在她密码中出现的所有单词“apple cow farmer banana bananas pies”，但是注意，字典中的单词可以不再密码中出现但密码中的单词一定在字典中。所以，Bessie的密码的两种可能是“applebananapies”和“applebananascow”，因为前一种字典序较前，故输出“applebananapies”。


现在，给你Bessie记得的字母和她的字典，求她的管理员密码。如果有多个答案，则输出字典序较小的那一个。


## 输入格式
\* Line 1: Two space-separated integers: L and NW

\* Line 2: A string of length L: P

\* Lines 3..NW+2: Line i+2 contains the ith word in the dictionary: W\_i

· 第一行：她密码的长度L和单词数量NW，用一个空格隔开


· 第二行：她所记得的密码字符串，没有多余空格


· 第三行到第NW+2行：单词Wi，一行一个单词


## 输出格式
\* Line 1: The lexicographically least password that fits

一行：Bessie的密码，不要有多余空格。


```input1
15 6 
a??l?ban??????? 
apple 
cow 
farmer 
banana 
bananas 
pies 

```

```output1
applebananapies 

```

## 提示
感谢@JJYZ\_cbh 提供翻译


