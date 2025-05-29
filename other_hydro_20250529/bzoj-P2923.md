## Description

Alphabet $A_k$ consists of $k$ initial letters of English alphabet. A positive integer called a weight is assigned to each letter of the alphabet. A weight of a word built from the letters of the alphabet $A_k$ is the sum of weights of all letters in this word. A language over an alphabet $A_k$ is any finite set of words built from the letters of this alphabet. A weight of a language is the sum of weights of all its words.

We say that the language is prefixless if for each pair of different words $w, v$ from this language $w$ is not a prefix of $v$. We want to find out what is the minimal possible weight of an $n$-element, prefixless language over an alphabet $A_k$.

Assume that $k = 2$, the weight of the letter $a ¡ª W(a) = 2$ and the weight of the letter b ¡ª W(b) = 5. Then the weight of the word ab ¡ª W(ab) = 2 + 5 = 7. W(aba) = 2 + 5 + 2 = 9. The weight of the language J = {ab, aba, b} ¡ª W(J) = 21. The language J is not prefixless, since the word ab is a prefix of aba. The lightest tree-element, prefixless language over the alphabet A2 (assuming that weights of the letters are as before) is {b, aa, ab}; its weight is 16.

Write a program that:

reads two integers n, k and the weights of k letters of an alphabet Ak from the standard input;
computes the minimal weight of a prefixless, n-element language over the alphabet Ak;
writes the result to the standard output.

## Input

In the first line of the standard input there are two positive integers n and k separated by a single space, (2 ¡Ü n ¡Ü 10,000, 2 ¡Ü k ¡Ü 26). These are the number of words in a language and the number of letters in an alphabet respectively. The second line contains k positive integers separated by single spaces. Each of them is not greater than 10,000. The i-th number is the weight of the i-th letter.

## Output

In the first and only line of the standard output there should be written one integer ¡ª the weight of the lightest prefixless n-element language over the alphabet Ak.

```input1
3 2
2 5
```
```output1 
16
```