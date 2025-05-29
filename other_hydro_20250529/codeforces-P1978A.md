## Description

<div><p>Alice has $n$ books. The $1$-st book contains $a_1$ pages, the $2$-nd book contains $a_2$ pages, $\ldots$, the $n$-th book contains $a_n$ pages. Alice does the following:</p><ul><li> She divides all the books into two non-empty piles. Thus, each book ends up in exactly one of the two piles.</li><li> Alice reads one book with the <span class="tex-font-style-bf">highest number</span> in each pile.</li></ul><p>Alice loves reading very much. Help her find the maximum total number of pages she can read by dividing the books into two piles.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 500$) �� the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 100$) �� the number of books Alice has.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) �� the number of pages in each book.</p></div><div class="output-specification"><p>For each test case, output a single integer �� the maximum number of pages Alice can read.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 500$) �� the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 100$) �� the number of books Alice has.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) �� the number of pages in each book.</p>

## Output

<p>For each test case, output a single integer �� the maximum number of pages Alice can read.</p>





```input1|2,3,6,7,10,11
5
2
1 1
4
2 3 3 1
5
2 2 3 2 2
2
10 3
3
1 2 3
```




```output1
2
4
5
13
5
```



## Note

<p>In the first test case, Alice can put book number $1$ in the first pile, and book number $2$ in the second pile. Then she will read $a_1 + a_2 = 1 + 1 = 2$ pages.</p><p>In the second test case, Alice can put books with numbers $2$ and $3$ in the first pile, and books with numbers $1$ and $4$ in the second pile. Then she will read the book with the highest number $3$ from the first pile, and the book with the highest number $4$ from the second pile. Then she will read $a_3 + a_4 = 3 + 1 = 4$ pages.</p>
