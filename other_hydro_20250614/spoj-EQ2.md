<p>Mr. B wrote an addition equation such as 123+321=444 on the blackboard after class. Mr. G removes some of the digits and makes it look like ¡°1?3+??1=44?¡±. After Mr. B realizes some digits are missing, he wants to recover them. Unfortunately, there may be more than one way to recover the equation. For example ¡°1?3+??1=44?¡± can be recovered to ¡°123+321=444¡± or ¡°143+301=444¡± and many other possible solutions. Your job is to determine the number of different possible solutions.</p>
<h3>Input</h3>
<p>Each test case describes a single line with an equation like <strong>a+b=c</strong> which contains exactly one plus sign <strong>+</strong> and one equal sign <strong>=</strong> with some digits are missing and replaced with <strong>?</strong>. You may assume <strong>a</strong>, <strong>b</strong> and <strong>c</strong> are non-negative integers, and the length of each number is no more than 9. In the other words, the equation will contain three integers less than 1,000,000,000.</p>
<h3>Output</h3>
<p>For each test case, display a single line with its case number and the number of possible solutions to recover the equation.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7+1?=1?
?1+?1=22

<strong>Output:</strong>
Case 1: 3
Case 2: 1
</pre>
<p><strong>Explanation</strong></p>
<p>There are three solutions for the first case:</p>
<p>7+10=17, 7+11=18, 7+12=19</p>
<p>There is only one solution for the second case:</p>
<p>11+11=22</p>
<p>Note that 01+21=22 is not a valid solution because extra leading zeros are not allowed.</p>