帕维尔发明了一个新游戏，这个游戏由一个有 $r$ 行 $c$ 列的整数矩阵构成，第 $p$ 行第 $q$ 列的整数为 $(p-1)\times c + q$。

现在他要开始按照下述规律重排这些数字，他称这个过程为“错乱矩阵”。

错乱矩阵的过程由一个 $(r-1)\times (c-1)$ 的矩阵定义，这个矩阵中只包含 $L,R$ 两种元素。
//咕咕咕了，这英语太长了也
Pavel garbles the matrix in a series of turns. On his first turn Pavel takes the number in the first row and the first column (it is put in parenthesis on the above picture for clarity) and writes it down.
Having written down the number he performs one garbling turn:
Pavel looks at the letter in the garbling map that corresponds to the position of the number he had just written down (one the first turn it is the letter in the upper-left corner). Depending on the letter in the garbling map the 2*2 block of the matrix whose upper-left corner contains the number he had just written (highlighted in the above picture) is rearranged in the following way: