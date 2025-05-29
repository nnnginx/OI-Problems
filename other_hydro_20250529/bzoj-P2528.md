## Description

Byteasar, the king of Bitotia, has ordained a reform of his subjects' names. The names of Bitotians often contain repeating phrases, e.g., the name `Abiabuabiab` has two occurrences of the phrase `abiab`. Byteasar intends to change the names of his subjects to sequences of bits matching the lengths of their original names. Also, he would very much like to reflect the original repetitions in the new names.

In the following, for simplicity, we will identify the upper- and lower-case letters in the names. For any sequence of characters (letters or bits) $W=W_1W_2\cdots W_k$ we say that the integer $P$ ($1\leq P < K$) is a period of $w$ if $W_i=W_{i+P}$ for all $i=1,\ \cdots,\ k-p$. We denote the set of all periods of $w$ by $\operatorname{Per}(w)$. For example, $\operatorname{Per}(\texttt{ABIABUABIAB})=\{6,\ 9\}$, $\operatorname{Per}(\texttt{01001010010})=\{5,\ 8,\ 10\}$, and $\operatorname{Per}(\texttt{0000})=\{1,\ 2,\ 3\}$.

Byteasar has decided that every name is to be changed to a sequence of bits that:

- has length matching that of the original name,
- has the same set of periods as the original name,
- is the smallest (lexicographically[^1]) sequence of bits satisfying the previous conditions.

[^1]: The sequence of bits $I_1I_2\cdots I_k$ is lexicographically smaller than the sequence of bits $Y_1Y_2\cdots Y_k$ if for some $i$, $1\leq i\leq k$, we have $I_i < Y_i$ and for all $j=1,\ \cdots,\ i-1$ we have $I_j=Y_j$.

For example, the name `ABIABUABIAB` should be changed to `01001101001`, `BABBAB` to `010010`, and `BABURBAB` to `01000010`.

Byteasar has asked you to write a program that would facilitate the translation of his subjects' current names into new ones. If you succeed, you may keep your current name as a reward!

## Input

In the first line of the standard input there is a single integer $k$ - the number of names to be translated ($1\leq k\leq 20$). The names are given in the following lines, one in each line. Each name consists of no less than and no more than $200000$ upper-case (capital) letters (of the English alphabet).

In the test worth $30\%$ of the points each name consists of at most $20$ letters.

## Output

Your program should print lines to the standard output. Each successive line should hold a sequence of zeroes and ones (without spaces in between) corresponding to the names given on the input. If an appropriate sequence of bits does not exists for some names, then `XXX` should be printed for that name.

```input1
3
ABIABUABIAB
BABBAB
BABURBAB
```

```output1
01001101001
010010
01000010
```

## Source

Thanks to Object022.