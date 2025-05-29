## 题意翻译

现在, 我们有一个由 $n$ 个单词组成的英文文本。但是它们都挤在一行里，单词间以一个半角空格分隔，就像丑陋的压行代码。你可以把他们通过 $k-1$ 次换行分割成 $k$ 行的文本并去除行首行末空格。为方便题意表述，我们以一个长度为 $k-1$ 的数列 $\{a_1,a_2,...,a_{k-1}\}$，表示第 $1$ 到第 $a_1$ 个单词放在第 $1$ 行，第 $a_1+1$到第$a_2$ 个单词放在第 $2$ 行，以此类推。

不过，为了让新的文本更加美妙，你希望**在满足每一行的长度不大于 $m$ 的情况下相邻行长度之差的和最小**。具体地，令 $\operatorname{length}(i) $表示第$i$个单词的长度，$\operatorname{line}(i)$ 表示第 $i$ 行的长度，则:

$$

\operatorname{line}(i)=(a_i-a_{i-1}-1)+\sum_{j=a_{i-1}+1}^{a_i}\operatorname{length}(j)

$$

你需要求得的答案 $Ans$ 为:

$$

Ans=\min_{k,\operatorname{line}(i)\le m}\{\sum_{i=1}^{k-1}|\operatorname{line}(i)-\operatorname{line}(i+1)|\}

$$

现在输入单词数 $n$，行长度限制 $m$ ，每个单词的长度 $\operatorname{length}(i)$，请输出答案。

## 输入格式

The first line of the standard input contains the numbers $m$ and $n$, $1\le m\le 10^6$,$1\le n\le 2\ 000$, separated by a single space. The second, last line of the standard input contains $n$ integers, denotingthe lengths of subsequent words, $1\le length(i)\le m$ for $i=1,2,\cdots,n$, separated by single spaces.



## 输出格式

The first and only line of the standard output should contain exactly one integer: the minimumcoefficient of aestheticism for those decompositions, whose every line's length does not exceed $m$.


```input1
6 4
4 3 2 5
```
```output1
3
```