<p><span style="white-space: normal;"><span style="font-size: small;">Numbers have feelings too! For any positive integer, take the sum of the squares of each of its digits, and add them together. Take the result, and do it again. A number is Happy if, after repeating this process a finite number of times, the sum is 1. Some happy numbers take more iterations of this process to get to 1 than others, and that would be referred to as its distance from happiness. 1¡¯s distance from happiness is 0. 23¡¯s distance from happiness is 3, since 2<sup>2</sup> + 3<sup>2</sup> = 13, 1<sup>2</sup> + 3<sup>2</sup> = 10, and 1<sup>2</sup> + 0<sup>2</sup> = 1. Numbers are Unhappy if they are infinitely far away from happiness because they get stuck in a loop.&nbsp;</span></span></p>
<p><span style="white-space: normal;"><span style="font-size: small;">Given the lower end and upper end of a range of integers, determine how many Unhappy numbers are in that range (inclusive).</span></span></p>
<h3><span style="font-size: 1.17em;">Input</span></h3>
<p><strong><span style="font-size: small;">There will be several test cases in the input. Each test case will consist of two positive integers, <strong>lo</strong> and <strong>hi</strong> (0&lt;<strong>lo</strong>¡Ü<strong>hi</strong>¡Ü10<sup>18</sup>) on a single line, with a single space between them. Input will terminate with two <strong>0</strong>s.</span></strong></p>
<h3><span style="font-size: 1.17em;">Output</span></h3>
<p>For each test case, output a single integer on its own line, indicating the count of Unhappy Numbers between <strong>lo</strong> and <strong>hi</strong> (inclusive). Output no extra spaces, and do not separate answers with blank lines.</p>
<h3><span style="font-size: 1.17em;">Example</span></h3>
<pre><span style="white-space: normal;">
<p><strong>Input:</strong>
<br>1 10 <br>1 100 <br>0 0
<br><br>
<strong>Output:</strong>
<br>7<br>80&nbsp;</p>
</span></pre>