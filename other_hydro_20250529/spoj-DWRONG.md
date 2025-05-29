<p>In elementary school, students learn to subtract fractions by first getting a common denominator and then subtracting the numerators. However, sometimes a student will work the problem incorrectly and still arrive at the correct answer. For example, for the problem</p>
<p>5/4 - 9/12</p>
<p>one can subtract the numbers in the numerator and then subtract the numbers in the denominator, simplify and get the answer. i.e.</p>
<p>5/4 - 9/12 = -4/-8 = 4/8 = 1/2</p>
<p>For a given fraction b/n, your task is to find all of the values a and m, where a¡Ý0 and m&gt;0, for which</p>
<p>a/m - b/n = (a-b)/(m-n)</p>
<h3>Input</h3>
<p>There will be several test cases in the input. Each test case will consist of a single line with two integers, b and n (1¡Üb,n¡Ü10<sup>6</sup>) separated by a single space. The input will end with a line with two 0s.</p>
<h3>Output</h3>
<p>For each case, output all of the requested fractions on a single line, sorted from smallest to largest. For equivalent fractions, print the one with the smaller numerator first. Output each fraction in the form ¡°a/m¡± with no spaces immediately before or after the ¡°/¡±. Output a single space between fractions. Output no extra spaces, and do not separate answers with blank lines.</p>
<h3>Example Input</h3>
<pre>9 12 <br>12 14 <br>4 12 <br>0 0</pre>
<h3>Example Output</h3>
<pre>0/24 5/20 8/16 8/8 5/4 <br>0/28 9/21 9/7 <br>0/24 3/18 3/6</pre>