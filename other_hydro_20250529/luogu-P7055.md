## 题目描述


According to Java standard library documentation, the hash code of String is computed as

$s[0] \times 31 ^ {n -1} + s[1] \times 31 ^ {n -2} + \cdots + s[n -1]$

Here $s[i]$ is the i-th character of the string, $n$ is the length of the string, and $^$ indicates exponentiation. Computation uses signed $32-bit$ integers in two's complement form.

Heather is going to hack the servers of Not Entirely Evil Recording Company $(NEERC).$ To perform an attack she needs $k$ distinct query strings that have equal hash codes. Unfortunately, NEERC servers accept query string containing lower- and uppercase English letters only.

Heather hired you to write a program that generates such query strings for her.



## 输入格式


The single line of the input file contains integer $k$ -- the number of required query strings to generate $(2 \le k \le 1000)$ .



## 输出格式


Output $k$ lines. Each line should contain a single query string. Each query string should be non-empty and its length should not exceed $1000$ characters. Query string should contain only lower- and uppercase English letters. All query strings should be distinct and should have equal hash codes.



## 题目大意
根据$Java$的标准库文件，字符串的哈希代码是这么计算的：

$$s[0]×31 ^{(n−1)}+s[1]×31^{(n−2)}+⋯+s[n−1]$$

在这里，s[i]指的是字符串中的第i位，n是字符串的长度。

这个计算过程用的是有符号的$32$位整数的二进制补码形式。

有一个人叫作 阖锕仄 $(Heather)$。他想要$hack$掉“不全是恶魔录音公司”$(NEERC)$。为了进行

一次攻击，阖锕仄需要$k$个有相同哈希代码的不同的询问字符串。不幸的是，$NEERC$的服务器

只接受只包含大小写字母的字符串。

阖锕仄请你帮忙写一个程序，以生成他需要的询问字符串。

-------

输入一个正整数$k$,代表需要的字符串的数量。

-------

输出有$k$行，每行的询问字符串都不应该为空，并且每行的字符串的长度应该小于等于1000个字符。

询问字符串的具体要求请看上文。

-------

时间限制：$2s$    

空间限制：$256MB$

翻译提供：@Trexmao

```input1
4

```

```output1
edHs
mENAGeS
fEHs
edIT

```

## 提示
Time limit: 2 s, Memory limit: 256 MB. 



