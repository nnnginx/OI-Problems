## 题目描述
Determined to discover the ancient mystery—the sound that the fox makes—you went into the forest, armed with a very good digital audio recorder. The forest is, however, full of animals’ voices, and on your recording, many different sounds can be heard. But you are well prepared for your task: you know exactly all the sounds which other animals make. Therefore the rest of the recording—all the unidentified noises—must have been made by the fox.

## 输入格式
The first line of input contains the number of test cases $T$. The descriptions of the test cases follow:

The first line of each test case contains the recording—words over lower case English alphabet, separated by spaces. Each contains at most 100 letters and there are no more than 100 words. The next few lines are your pre-gathered information about other animals, in the format <animal> goes <sound>. There are no more than 100 animals, their names are not longer than 100 letters each and are actual names of animals in English. There is no fox goes ... among these lines.

The last line of the test case is exactly the question you are supposed to answer: what does the fox say?

## 输出格式
For each test case, output one line containing the sounds made by the fox, in the order from the recording. You may assume that the fox was not silent (contrary to popular belief, foxes do not communicate by Morse code).

## 题目大意
### 题目大意

森林里面有很多声响，你想知道有哪些声响是由狐狸发出来的。

已知你搜集到了 $n$ 个声响，并且还知道某些其他动物能够发出的声响，已知如果没有哪一个声响是由其他任何一种动物发出来的话，那这个声响绝对是由狐狸发出来的。现在，给定你这 $n$ 个声响，以及某些其他动物能够发出的声响，请你求出狐狸发出的声响。

### 输入格式
**本题有多组询问。**

第一行包含一个整数 $T$，表示数据的组数。  
接下来若干组数据，每组数据由三部分组成：

- 第一行 $n$ 个仅由小写字母组成的字符串，代表搜集到的 $n$ 个声响。
- 接下来有若干行，代表某些其他动物能够发出的声响。格式为 ``<animal> goes <sound>``，其中 `<animal>` 代表动物的名称（仅由一个字符串组成），`<sound>` 代表这个动物发出的声响（仅由一个字符串组成）。保证不会在这些动物中出现狐狸。
- 最后一行，一个确定的字符串 ``what does the fox say?``。

### 输出格式
对于每组数据，输出仅一行，代表狐狸能够发出的声响。

### 数据范围
$n\leqslant 100$。  
保证每个字符串的长度不超过 $100$。

Translated by Eason_AC  
2020.10.30

```input1
1
toot woof wa ow ow ow pa blub blub pa toot pa blub pa pa ow pow toot
dog goes woof
fish goes blub
elephant goes toot
seal goes ow
what does the fox say?

```

```output1
wa pa pa pa pa pa pow

```

## 提示
Time limit: 1000 ms, Memory limit: 1048576 kB. 

 Central Europe Regional Contest (CERC) 2013

