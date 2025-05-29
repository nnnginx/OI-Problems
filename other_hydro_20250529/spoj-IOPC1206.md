<p align="justify">Consider integers N and K such that 2 ¡Ü K ¡Ü N. Write all the numbers 0 ¡Ü i &lt; N in base K, adding leading zeros where necessary so that all the numbers are of equal length in base K. The score of an integer i (0 ¡Ü i &lt; N) in the list is defined in the following fashion : Consider the first digit of i in base K. Count the total number of times this digit occurs as first digit of some integer in the list. This is the score of the first digit of i. The number of times the second digit of i appears as the second digit of some integer in the list is the score of the second digit of i, and so on. The sum of scores of all digits of i is the score of i.</p>
<p align="justify">As an example, suppose N=4 and K=3. Then the numbers in the list are 00,01,02 and 10. Let us find the score of i=00. The first digit of i appears as the first digit thrice (00,01,02) and the second digit of i appears as second digit twice (00,10). Thus the score of 00 is 3+2=5.</p>
<p align="justify">An integer K (2 ¡Ü K ¡Ü N) is called a fair base of N if the scores of all i (0 ¡Ü i &lt; N) are equal for base K. The number of fair bases in the range 2 ¡Ü K ¡Ü N is termed the fairness factor of the integer N.</p>
<p align="justify">Given integers a and b (2 ¡Ü a ¡Ü b ¡Ü 10<sup>12</sup>), find the sum of fairness factors of all i such that a ¡Ü i ¡Ü b.</p>
<h3>Input</h3>
<p align="justify">The first line of input contains T, the number of test cases (T ¡Ü 20). Following these are T lines, each containing two space separated integers a and b (2 ¡Ü a ¡Ü b ¡Ü 10<sup>12</sup>).</p>
<h3>Output</h3>
<p align="justify">For each (a,b) pair in the input, output the sum of fairness factors of i in the range a ¡Ü i ¡Ü b.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
4 8
20 30

<strong>Output:</strong>
9
27
</pre>