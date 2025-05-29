<p>The director of a new movie needs to create a scaled set for the  movie. In the set there will be N skyscrapers, with distinct integer  heights from 1 to N meters. The skyline will be determined by the  sequence of the heights of the skyscrapers from left to right. It will  be a permutation of the integers from 1 to N.</p>
<p>The director is  extremely meticulous, so she wants to avoid a certain sloping pattern.  She doesn¡¯t want for there to be ANY three buildings in positions i, j  and k, i &lt; j &lt; k, where the height of building i is smaller than  that of building j, and building j¡¯s height is smaller than building k¡¯s  height.</p>
<p>Your task is to tell the director, for a given number of  buildings, how many distinct orderings for the skyline avoid the sloping  pattern she doesn't like.</p>
<h3>Input</h3>
<p>There will be several test cases in the input. Each test case will  consist of a single line containing a single integer N (3 ¡Ü N ¡Ü 1,000),  which represents the number of skyscrapers. The heights of the  skyscrapers are assumed to be 1, 2, 3, ..., N. The input will end with a  line with a single 0.</p>
<h3>Output</h3>
<p>For each test case, output a single integer, representing the number  of good skylines - those avoid the sloping pattern that the director  dislikes - modulo 1,000,000. Print each integer on its own line with no  spaces. Do not print any blank lines between answers.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>4<br>0<br><br><strong>Output:</strong><br>5<br>14<br></pre>