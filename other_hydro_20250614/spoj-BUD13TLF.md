<p>Given n boxes with widths of w1, w2, . . . , wn and another big box with width W, find how many ways the boxes can be put in the big box. The constrains are:</p>
<p>1) Of course the summation of widths of the placed boxes should not be greater than W.</p>
<p>2) The boxes should be placed one by one starting from left without leaving any empty spaces between them. So, the end of the big box may contain empty spaces. But if there is any unplaced box which can be fit in this space, the ordering should be considered invalid (See the explanation for sample case 1).</p>
<p>3) Two orderings are considered different if in one ordering, one box is in i-th position, but in another ordering, it isn¡¯t.</p>
<p>4) If two boxes have same widths, they should be considered same</p>
<h3>Input</h3>
<p>Input starts with an integer T (¡Ü 100), denoting the number of test cases.</p>
<p>Each case starts two integers n (1 ¡Ü n ¡Ü 100) and W (1 ¡Ü W ¡Ü 1000). The next line contains n space separated integers, denoting w1 w2 . . . wn (1 ¡Ü wi ¡Ü W).</p>
<h3>Output</h3>
<p>For each case, print the case number first and the result modulo 10007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 5
1 2 3
5 10
1 2 2 4 5

<strong>Output:</strong>
Case 1: 6
Case 2: 30

<strong>Notes:</strong>&nbsp;For the first case of the Sample Input, the orderings are
12
13
21
23
31
32
Only 1 or 2 or 3 is not solutions since we can still place another box.</pre>