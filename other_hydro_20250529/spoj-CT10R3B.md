<p>We are looking into building a very long fence. We have already found a  nice place to build it, and all that remains is to collect the  materials.</p>
<p>From local hardware stores, we can buy unlimited numbers of wooden  boards, each of which can come in a variety of different lengths. To  avoid waste, we want to make sure that the total length of these boards  is <em>exactly</em> equal to the length of the fence we are trying to  build.</p>
<p>Given the length of the fence, and the possible board lengths that we  can use, what is the minimum number of boards that we need to purchase  in order to get exactly the right length?</p>
<p><em>Beware:</em> the fence is going to be very long!</p>
<h3>Input</h3>
<p>The first line of the input file contains the number of cases, <strong>T</strong>.  <strong>T</strong> test cases follow.</p>
<p>Each test case consists of two lines. The first line contains  space-separated integers <strong>L</strong> and <strong>N</strong>. These represent the  total length of the fence, and the number of different board lengths  that can be purchased. The second line contains <strong>N</strong> space-separated  integers <strong>B<sub>1</sub></strong>, <strong>B<sub>2</sub></strong>, ..., <strong>B<sub>N</sub></strong>,  representing all the possible board lengths.</p>
<h3>Output</h3>
<p>For each test case, output one line containing "Case #x: M", where x is  the case number (starting from 1) and M is as follows:</p>
<ul>
<li> If it is possible to purchase one or more boards so that their  total length is exactly equal to <strong>L</strong>, then M should be the minimum  number of boards required to do this. </li>
<li> Otherwise, M should be the string "IMPOSSIBLE". </li>
</ul>
<h3>Limits</h3>
<p>1 �� <strong>T</strong> �� 50.<br> 10<sup>10</sup> �� <strong>L</strong> �� 10<sup>18</sup>.</p>
<p>1 �� <strong>N</strong> �� 100.</p>
<p>1 �� <strong>B<sub>i</sub></strong> �� 100000.</p>
<p>All the <strong>B<sub>i</sub></strong> values in a single test case are distinct.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><code>2<br> 10000000001 3<br> 23 51 100<br> 10000000001 3<br> 100 52 22 </code><br><strong>Output:</strong><br><code>Case #1: 100000004<br>Case #2: IMPOSSIBLE<br><br><br></code></pre>