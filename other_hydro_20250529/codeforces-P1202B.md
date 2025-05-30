## Description

<div><p>Suppose you have a special $x$-$y$-counter. This counter can store some value as a decimal number; at first, the counter has value $0$. </p><p>The counter performs the following algorithm: it prints its lowest digit and, after that, adds either $x$ or $y$ to its value. So all sequences this counter generates are starting from $0$. For example, a $4$-$2$-counter can act as follows:</p><ol> <li> it prints $0$, and adds $4$ to its value, so the current value is $4$, and the output is $0$; </li><li> it prints $4$, and adds $4$ to its value, so the current value is $8$, and the output is $04$; </li><li> it prints $8$, and adds $4$ to its value, so the current value is $12$, and the output is $048$; </li><li> it prints $2$, and adds $2$ to its value, so the current value is $14$, and the output is $0482$; </li><li> it prints $4$, and adds $4$ to its value, so the current value is $18$, and the output is $04824$. </li></ol><p>This is only one of the possible outputs; for example, the same counter could generate $0246802468024$ as the output, if we chose to add $2$ during each step.</p><p>You wrote down a printed sequence from one of such $x$-$y$-counters. But the sequence was corrupted and several elements from the sequence could be erased.</p><p>Now you'd like to recover data you've lost, but you don't even know the type of the counter you used. You have a decimal string $s$ �� the remaining data of the sequence. </p><p>For all $0 \le x, y &lt; 10$, calculate the minimum number of digits you have to insert in the string $s$ to make it a possible output of the $x$-$y$-counter. Note that you can't change the order of digits in string $s$ or erase any of them; only insertions are allowed.</p></div><div class="input-specification"><p>The first line contains a single string $s$ ($1 \le |s| \le 2 \cdot 10^6$, $s_i \in \{\text{0} - \text{9}\}$) �� the remaining data you have. It's guaranteed that $s_1 = 0$.</p></div><div class="output-specification"><p>Print a $10 \times 10$ matrix, where the $j$-th integer ($0$-indexed) on the $i$-th line ($0$-indexed too) is equal to the minimum number of digits you have to insert in the string $s$ to make it a possible output of the $i$-$j$-counter, or $-1$ if there is no way to do so.</p></div>

## Input

<p>The first line contains a single string $s$ ($1 \le |s| \le 2 \cdot 10^6$, $s_i \in \{\text{0} - \text{9}\}$) �� the remaining data you have. It's guaranteed that $s_1 = 0$.</p>

## Output

<p>Print a $10 \times 10$ matrix, where the $j$-th integer ($0$-indexed) on the $i$-th line ($0$-indexed too) is equal to the minimum number of digits you have to insert in the string $s$ to make it a possible output of the $i$-$j$-counter, or $-1$ if there is no way to do so.</p>

## Samples

```input1
0840
```

```output1
-1 17 7 7 7 -1 2 17 2 7 
17 17 7 5 5 5 2 7 2 7 
7 7 7 4 3 7 1 7 2 5 
7 5 4 7 3 3 2 5 2 3 
7 5 3 3 7 7 1 7 2 7 
-1 5 7 3 7 -1 2 9 2 7 
2 2 1 2 1 2 2 2 0 1 
17 7 7 5 7 9 2 17 2 3 
2 2 2 2 2 2 0 2 2 2 
7 7 5 3 7 7 1 3 2 7
```




## Note

<p>Let's take, for example, $4$-$3$-counter. One of the possible outcomes the counter could print is $0(4)8(1)4(7)0$ (lost elements are in the brackets).</p><p>One of the possible outcomes a $2$-$3$-counter could print is $0(35)8(1)4(7)0$.</p><p>The $6$-$8$-counter could print exactly the string $0840$.</p>
