## Description

<div><p>There are $n$ candies in a row, they are numbered from left to right from $1$ to $n$. The size of the $i$-th candy is $a_i$.</p><p>Alice and Bob play an interesting and tasty game: they eat candy. Alice will eat candy <span class="tex-font-style-bf">from left to right</span>, and Bob ！ <span class="tex-font-style-bf">from right to left</span>. The game ends if all the candies are eaten.</p><p>The process consists of moves. During a move, the player eats one or more sweets from her/his side (Alice eats from the left, Bob ！ from the right).</p><p>Alice makes the first move. During the first move, she will eat $1$ candy (its size is $a_1$). Then, each successive move the players alternate ！ that is, Bob makes the second move, then Alice, then again Bob and so on.</p><p>On each move, a player counts the total size of candies eaten during the current move. Once this number becomes strictly greater than the total size of candies eaten by the other player on their previous move, the current player stops eating and the move ends. In other words, on a move, a player eats the smallest possible number of candies such that the sum of the sizes of candies eaten on this move is <span class="tex-font-style-bf">strictly greater</span> than the sum of the sizes of candies that the other player ate on the <span class="tex-font-style-bf">previous</span> move. If there are not enough candies to make a move this way, then the player eats up all the remaining candies and the game ends.</p><p>For example, if $n=11$ and $a=[3,1,4,1,5,9,2,6,5,3,5]$, then:</p><ul> <li> move 1: Alice eats one candy of size $3$ and the sequence of candies becomes $[1,4,1,5,9,2,6,5,3,5]$. </li><li> move 2: Alice ate $3$ on the previous move, which means Bob must eat $4$ or more. Bob eats one candy of size $5$ and the sequence of candies becomes $[1,4,1,5,9,2,6,5,3]$. </li><li> move 3: Bob ate $5$ on the previous move, which means Alice must eat $6$ or more. Alice eats three candies with the total size of $1+4+1=6$ and the sequence of candies becomes $[5,9,2,6,5,3]$. </li><li> move 4: Alice ate $6$ on the previous move, which means Bob must eat $7$ or more. Bob eats two candies with the total size of $3+5=8$ and the sequence of candies becomes $[5,9,2,6]$. </li><li> move 5: Bob ate $8$ on the previous move, which means Alice must eat $9$ or more. Alice eats two candies with the total size of $5+9=14$ and the sequence of candies becomes $[2,6]$. </li><li> move 6 (the last): Alice ate $14$ on the previous move, which means Bob must eat $15$ or more. It is impossible, so Bob eats the two remaining candies and the game ends. </li></ul><p>Print the number of moves in the game and two numbers:</p><ul> <li> $a$ ！ the total size of all sweets eaten by Alice during the game; </li><li> $b$ ！ the total size of all sweets eaten by Bob during the game. </li></ul></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 5000$) ！ the number of test cases in the input. The following are descriptions of the $t$ test cases.</p><p>Each test case consists of two lines. The first line contains an integer $n$ ($1 \le n \le 1000$) ！ the number of candies. The second line contains a sequence of integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 1000$) ！ the sizes of candies in the order they are arranged from left to right.</p><p>It is guaranteed that the sum of the values of $n$ for all sets of input data in a test does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each set of input data print three integers ！ the number of moves in the game and the required values $a$ and $b$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 5000$) ！ the number of test cases in the input. The following are descriptions of the $t$ test cases.</p><p>Each test case consists of two lines. The first line contains an integer $n$ ($1 \le n \le 1000$) ！ the number of candies. The second line contains a sequence of integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 1000$) ！ the sizes of candies in the order they are arranged from left to right.</p><p>It is guaranteed that the sum of the values of $n$ for all sets of input data in a test does not exceed $2\cdot10^5$.</p>

## Output

<p>For each set of input data print three integers ！ the number of moves in the game and the required values $a$ and $b$.</p>

## Samples

```input1
7
11
3 1 4 1 5 9 2 6 5 3 5
1
1000
3
1 1 1
13
1 2 3 4 5 6 7 8 9 10 11 12 13
2
2 1
6
1 1 1 1 1 1
7
1 1 1 1 1 1 1
```

```output1
6 23 21
1 1000 0
2 1 2
6 45 46
2 2 1
3 4 2
4 4 3
```



