<p>Grimm's conjecture states that to each element of a set of consecutive composite numbers one can assign a distinct prime that divides it.</p>
<p>For example, for the range 242 to 250, one can assign distinct primes as follows:</p>
<p style="text-align: center;"><img src="../../../content/joshkirstein:666" alt="" width="596" height="63"></p>
<p style="text-align: left;">Given the lower and upper bounds of a sequence of composite numbers, find a distinct prime for each. If there is more than one such assignment, output the one with the smallest first prime. If there is still more than one, output the one with the smallest second prime, and so on.</p>
<h3>Input</h3>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There will be several test cases in the input. Each test case will consist of a single line</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">with two integers, lo and hi (4¡Ülo&lt;hi¡Ü1010</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">), separated by a single space. It is guaranteed</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">that all the numbers in the range from lo to hi inclusive are composite. The input will</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">end with a line with two 0s.</div>
<p>There will be several test cases in the input. Each test case will consist of a single line with two integers, lo and hi (4¡Ülo&lt;hi¡Ü10<sup>10</sup>), separated by a single space. It is guaranteed that all the numbers in the range from lo to hi inclusive are composite. The input will end with a line with two 0s.</p>
<h3>Output</h3>
<p>For each test case, output the set of unique primes, in order, all on the same line, separated by single spaces. Output no extra spaces, and do not separate answers with blank lines.</p>
<h3>Example Input</h3>
<pre>242 250
8 10
0 0</pre>
<h3>Example Output</h3>
<pre>2 3 61 7 41 13 31 83 5
2 3 5</pre>
<p>&nbsp;</p>