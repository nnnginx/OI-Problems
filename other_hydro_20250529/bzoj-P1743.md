## 题目描述

Farmer John has set up a puzzle for his cows to solve. At the entrance to the barn, he has laid out an $h \times w \ (1 \le  h \le  30, 1 \le  w \le  30)$ grid of letters. Before a cow can enter the barn, she must spell out a valid English word by jumping from square to square, creating a sequence of letters. She can start at any square but may only jump to a subsequent square that is located to the right and/or above the current square (i. e., neither to the left nor lower). The next square can be any distance from the current one since the cows are world-class jumpers!No two cows may traverse the exact same path, although two cows are allowed to spell the same word via different paths. As an example, consider this grid (presuming'TO'and'OX'are words): T X X O T X Q T X T X Q Four paths are valid, all spelling'TO' (one spelling requires a'T'from the bottom row and an'O'from the top row).'OX'is a valid word, but would require jumping to an'X'square left of the'O', which is not allowed. Given the grid and a list of valid words, compute the number of cows that can enter the barn without any cow repeating a path. The file'dict. txt'will be available and will contain the list of valid words, one per line. See a copy of it at http//ace.delos.com/usaco/dict-twalk.txt.

## 输入格式

* Line $1$: Two integers: $h$ and $w$.
* Lines $2\dots h+1$: Each line contains $w$ characters, without spaces, representing a row in the grid. The first row is the top row. The first character in each row is the left-most character.

## 输出格式

* Line $1$: The number of cows that can enter the barn without repeating a path.

```input1
3 4
TXXO
TXQT
XTXQ
```
```output1
4
```
## 样例说明

OUTPUT DETAILS:   
$4$ cows can enter the barn, each one spelling out one of the'TO's.

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le  h \le  30, 1 \le  w \le  30$。

## 题目来源
Gold