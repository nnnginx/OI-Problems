## 题目描述
As practice will tell you, the English rules for comma placement are complex, frustrating, and often ambiguous. Many people, even the English, will, in practice, ignore them, and, apply custom rules, or, no rules, at all.

Doctor Comma Sprinkler solved this issue by developing a set of rules that sprinkles commas in a sentence with no ambiguity and little simplicity. In this problem you will help Dr. Sprinkler by producing an algorithm to automatically apply her rules.

Dr. Sprinkler's rules for adding commas to an existing piece of text are as follows:

If a word anywhere in the text is preceded by a comma, find all occurrences of that word in the text, and put a comma before each of those occurrences, except in the case where such an occurrence is the first word of a sentence or already preceded by a comma.

If a word anywhere in the text is succeeded by a comma, find all occurrences of that word in the text, and put a comma after each of those occurrences, except in the case where such an occurrence is the last word of a sentence or already succeeded by a comma.

Apply rules $1$ and $2$ repeatedly until no new commas can be added using either of them.

As an example, consider the text

please sit spot. sit spot, sit. spot here now here.

Because there is a comma after spot in the second sentence, a comma should be added after spot in the third sentence as well (but not the first sentence, since it is the last word of that sentence). Also, because there is a comma before the word sit in the second sentence, one should be added before that word in the first sentence (but no comma is added before the word sit beginning the second sentence because it is the first word of that sentence). Finally, notice that once a comma is added after spot in the third sentence, there exists a comma before the first occurrence of the word here. Therefore, a comma is also added before the other occurrence of the word here. There are no more commas to be added so the final result is

please, sit spot. sit spot, sit. spot, here now, here.



## 输入格式


The input contains one line of text, containing at least $2$ characters and at most $1 000 000$ characters. Each character is either a lowercase letter, a comma, a period, or a space. We define a word to be a maximal sequence of letters within the text. The text adheres to the following constraints:

The text begins with a word.

Between every two words in the text, there is either a single space, a comma followed by a space, or a period followed by a space (denoting the end of a sentence and the beginning of a new one).

The last word of the text is followed by a period with no trailing space.



## 输出格式


Display the result after applying Dr. Sprinkler's algorithm to the original text.



## 题目大意
给定一些文本，对他添加逗号。

添加的规则为：

1. 找到一个单词前面有逗号，就在文本中的其他这个单词前添加一个逗号，除非这个单词是句子的第一个单词，或单词前已经有逗号了。
2. 找到一个单词后面有逗号，就在文本中的其他这个单词后添加一个逗号，除非这个单词是句子的最后一个单词，或单词后已经有逗号了。
3. 重复 1 和 2 直到不能填加逗号。

$2 \le $ 文本长度 $ \le 10^6$。

文本满足以下特征：

- 文本开头为一个单词；
- 两个单词之间为一个空格，或者一个逗号一个空格，或者一个句号一个空格；
- 文本末尾为一个句号。

翻译者：一只书虫仔

```input1
please sit spot. sit spot, sit. spot here now here.

```

```output1
please, sit spot. sit spot, sit. spot, here now, here.

```

```input2
one, two. one tree. four tree. four four. five four. six five.

```

```output2
one, two. one, tree. four, tree. four, four. five, four. six five.

```

## 提示
Time limit: 8 s, Memory limit: 1024 MB. 



