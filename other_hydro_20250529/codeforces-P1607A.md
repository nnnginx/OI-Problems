## Description

<div><p>You are given a keyboard that consists of $26$ keys. The keys are arranged sequentially in one row in a certain order. Each key corresponds to a unique lowercase Latin letter.</p><p>You have to type the word $s$ on this keyboard. It also consists only of lowercase Latin letters.</p><p>To type a word, you need to type all its letters consecutively one by one. To type each letter you must position your hand exactly over the corresponding key and press it.</p><p>Moving the hand between the keys takes time which is equal to the absolute value of the difference between positions of these keys (the keys are numbered from left to right). No time is spent on pressing the keys and on placing your hand over the first letter of the word.</p><p>For example, consider a keyboard where the letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>' are arranged in consecutive alphabetical order. The letters '<span class="tex-font-style-tt">h</span>', '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">l</span>' and '<span class="tex-font-style-tt">o</span>' then are on the positions $8$, $5$, $12$ and $15$, respectively. Therefore, it will take $|5 - 8| + |12 - 5| + |12 - 12| + |15 - 12| = 13$ units of time to type the word "<span class="tex-font-style-tt">hello</span>". </p><p>Determine how long it will take to print the word $s$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;�� the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases.</p><p>The first line of a description contains a keyboard&nbsp;�� a string of length $26$, which consists only of lowercase Latin letters. Each of the letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>' appears exactly once on the keyboard.</p><p>The second line of the description contains the word $s$. The word has a length from $1$ to $50$ letters inclusive and consists of lowercase Latin letters.</p></div><div class="output-specification"><p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to the test case is the minimal time it takes to type the word $s$ on the given keyboard.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;�� the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases.</p><p>The first line of a description contains a keyboard&nbsp;�� a string of length $26$, which consists only of lowercase Latin letters. Each of the letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>' appears exactly once on the keyboard.</p><p>The second line of the description contains the word $s$. The word has a length from $1$ to $50$ letters inclusive and consists of lowercase Latin letters.</p>

## Output

<p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to the test case is the minimal time it takes to type the word $s$ on the given keyboard.</p>

## Samples

```input1
5
abcdefghijklmnopqrstuvwxyz
hello
abcdefghijklmnopqrstuvwxyz
i
abcdefghijklmnopqrstuvwxyz
codeforces
qwertyuiopasdfghjklzxcvbnm
qqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqq
qwertyuiopasdfghjklzxcvbnm
abacaba
```

```output1
13
0
68
0
74
```



