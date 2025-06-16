<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Background</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">In 1949 the Indian mathematician D.R. Kaprekar discovered a class of numbers called&nbsp;<em>self-numbers</em>. For any positive integer&nbsp;<em>n</em>, define&nbsp;<em>d(n)</em>&nbsp;to be<em>n</em>&nbsp;plus the sum of the digits of&nbsp;<em>n</em>. (The&nbsp;<em>d</em>&nbsp;stands for&nbsp;<em>digitadition</em>, a term coined by Kaprekar.) For example:</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">&nbsp;</p>
<p>d(75) = 75 + 7 + 5 = 87</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">&nbsp;</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">Given any positive integer n as a starting point, you can construct the infinite increasing sequence of integers&nbsp;<em>n, d(n), d(d(n)), d(d(d(n))), ...</em>&nbsp;For example, if you start with 33, the next number is 33 + 3 + 3 = 39, the next is 39 + 3 + 9 = 51, the next is 51 + 5 + 1 = 57, and so you generate the sequence</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">&nbsp;</p>
<p>33, 39, 51, 57, 69, 84, 96, 111, 114, 120, 123, 129, 141, ...</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">&nbsp;</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">The number&nbsp;<em>n</em>&nbsp;is called a&nbsp;<em>generator</em>&nbsp;of&nbsp;<em>d(n)</em>. In the sequence above, 33 is a generator of 39, 39 is a generator of 51, 51 is a generator of 57, and so on.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">Some numbers have more than one generator: For example, 101 has two generators, 91 and 100. A number with no generators is a&nbsp;<em>self-number</em>. There are thirteen self-numbers less than 100: 1, 3, 5, 7, 9, 20, 31, 42, 53, 64, 75, 86, and 97.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Problem</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">Write a program to output all positive self-numbers less than 1000000 in increasing order, one per line.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Input</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">There is no input.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Output</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">All positive self-numbers less than 1000000 in increasing order, one per line.</p>