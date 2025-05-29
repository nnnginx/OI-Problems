## 题目描述

Like all bovines，Farmer John's cows speak the peculiar 「Cow」 language．Like so many languages，each word in this language comprises a sequence of upper and lowercase letters （$\text{A}\sim\text{Z}$ and $\text{a}\sim \text{z}$）．A word is valid if and only if each ordered pair of adjacent letters in the word is a valid pair．

Farmer John，ever worried that his cows are plotting against him，recently tried to eavesdrop on their conversation．He overheard one word before the cows noticed his presence．The Cow language is spoken so quickly，and its sounds are so strange，that all that Farmer John was able to perceive was the total number of uppercase letters，$U$ and the total number of lowercase letters，$L$ in the word．

Farmer John knows all $P$ valid ordered pairs of adjacent letters．He wishes to know how many different valid words are consistent with his limited data．However，since this number may be very large，he only needs the value modulo $97654321$．

约翰的奶牛讲的是别人听不懂的「牛语」。牛语使用的字母就是英文字母，有大小写之分。牛语中存在 $P$ 个合法的词素，每个词素都由两个字母组成。牛语的单词是由字母组成的序列，一个单词是有意义的充要条件是任意相邻的字母都是合法的词素。

约翰担心他的奶牛正在密谋反对他，于是最近一直在偷听他们的对话。可是，牛语太复杂了，他模模糊糊地只听到了一个单词，并确定了这个单词中有 $U$ 个大写字母，$L$ 个小写字母。现在他想知道，如果这个单词是有意义的，那么有多少种可能性呢？由于这个数字太大了，你只要输出答案取 $97654321$ 的余数就可以了。

## 输入格式

* Line $1$：Three space-separated integers：$U,L$ and $P$

* Lines $2 \dots P + 1$：Two letters （each of which may be uppercase or lowercase），representing one valid ordered pair of adjacent letters in Cow．

**第一行：三个用空格隔开的整数：**$U,L$ **和** $P$**。**

**第二行到** $P + 1$ **行：第** $i + l$ **有两个字母，表示第** $i$ **个词素，没有两个词素是完全相同的。**

## 输出格式

* Line $1$：A single integer，the number of valid words consistent with Farmer John's data mod $97654321$．

单个整数，表示符合条件的单词数量除以 $97654321$ 的余数。

```input1
2 2 7
AB
ab
BA
ba
Aa
Bb
bB
```

```output1
7
```

## 样例解释1

INPUT DETAILS：  
The word Farmer John overheard had $2$ uppercase and $2$ lowercase letters．The valid pairs of adjacent letters are $AB,ab,BA,ba,Aa,Bb$ and $bB$．

可能的单词为 $\text{AabB，Abba，abBA，BAab，BbBb，bBAa，bBbB}$ 共 $7$ 个。

## 题目来源

Gold

## 数据规模与约定

$100\%$ 的数据满足：$1 \le U,L \le 250$，$1 \le P \le 200$。
