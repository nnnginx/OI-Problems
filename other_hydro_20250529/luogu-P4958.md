## 题目描述
Little Mate got an array of lowercase letters from the English alphabet as a present from his
parents. In order to have at least some use of such a clever present, he decided to use it for
finding rhymes when writing his next song.

To find a specific rhyme, Mate wants to select a word of length D that ends with an array of
characters XY, i.e. where the next to last letter is X, and the last Y. Mate’s process of
selecting a word is by first crossing out some letters in a given sequence, and then merging
the letters he didn’t cross out into a single word. He wants to know in how many different
ways he can cross out the letters so that he meets the given conditions.

The selection of two words is considered distinct if the sets of positions of the crossed-out
letters are different.


## 输入格式
The first line of input contains an array of lowercase letters of the English alphabet S (2 ≤ |S|
≤ 2000).

The second line of input contains the integer Q (1 ≤ Q ≤ 500 000), the number of different
rhymes for which Mate needs to select words.

Each of the following Q lines contains the integer D (2 ≤ D ≤ |S|) and an array of lowercase
letters of the English alphabet XY from the task.

## 输出格式
The $i^{th}$ out of Q lines must contain the required number of ways for the $i^{th}$ rhyme. Since that number can be quite large, output only the value **modulo 1 000 000 007​**.

## 题目大意
给定一个字符串 $S$，一共有 $Q$ 个询问，每一个询问给定一个数字 $N$ 和 两个字符 $A$ 和 $B$，问你在 $S$ 中有多少长度为 $N$ 的子串为 $A, B$ 结尾，其中 $A$ 为倒数第二个字符，$B$ 为最后一个字符。注意，选取的字母可以不连续。

```input1
banana
3
2 na
3 ba
4 nn
```

```output1
3
0
1
```

```input2
malimateodmameitate
3
10 ot
7 aa
3 me
```

```output2
2
464
56
```

## 提示
In test cases worth 40% of total points, it will hold |S| ≤ 50.

In test cases worth an additional 40% of total points, it will hold |S| ≤ 200.

**Clarification of the first test case:**

Word of length 2 that ends with “na” can be obtained in the following ways:

~~b a n a~~$\ $**n a**​, ~~b a~~$\ $**n a**$\ $~~​n a~~, ~~b a~~$\ $**n**​ ~~a n~~$\ $**a**

