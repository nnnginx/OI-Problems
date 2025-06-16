<p>Manoj is a geek who loves ciphering data. He is also known for doing stupid things like setting fire in his room like a caveman. One day he does that and accidentally throws a paper containing some sensitive information. However, he has the encrypted version of the data.&nbsp;</p>
<p>Each number in the original text is the number of pairs of integers <strong>A</strong>,<strong>B (A&lt;B, 1 &lt;= A,B &lt;= N)</strong>&nbsp;such that their GCD Quotients match the given set of integers.</p>
<p>GCD Quotients of a pair <strong>(A,B)</strong>&nbsp;is defined as the sequence of quotients that are obtained while computing the gcd of <strong>A</strong> and <strong>B </strong><strong>using Euclid's Algorithm</strong>. For example,&nbsp;</p>
<pre><div id="_mcePaste" style="position: absolute; left: -10000px; top: 90px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; GCD(7,9) =&nbsp;</div>          GCD(7,9) = 
              7) 9 (<strong>1</strong>
                 7
                ---
                 2) 7 (<strong>3</strong>
                    6
                   ---
                    1) 2 (<strong>2</strong>
                       2
                      ---
                       0
                      ---</pre>
<p>In the above example, the gcd quotient sequence is <strong>[1,3,2]</strong>.&nbsp;</p>
<h3>Input</h3>
<p>The first line contains <strong>T</strong>, the number of test cases. Each test case contains two integers <strong>N</strong>&nbsp;and <strong>Q</strong>&nbsp;on the first line and <strong>Q </strong>integers on the second line, denoting the quotient sequence.</p>
<h3>Output</h3>
<p>For each test case, output the number of pairs of integers, whose gcd quotient sequence match with the given sequence.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>10 3</pre>
<pre>1 3 2</pre>
<pre>2 1</pre>
<pre>3

<strong>Output:</strong>

</pre>
<pre>1</pre>
<pre>0</pre>
<pre><strong>Explaination:</strong></pre>
<pre>For the first case, there exists only one such pair in the range [1,10], which is (7,9).&nbsp;</pre>
<pre>For the second case,&nbsp;the smallest possible pair is (1,3), but since the given range is only [1,2],</pre>
<pre>hence we have zero such pairs.</pre>
<pre><strong>Constraints:</strong></pre>
<pre>1 &lt;= N &lt;= 10<sup>16</sup></pre>
<pre>1 &lt;= Q &lt;= 50</pre>
<pre>1 &lt;= each quotient value &lt;= 1000</pre>
<pre>1 &lt;= T &lt;= 10<sup>5</sup></pre>
<pre>Product of all Quotient Values &lt;= 10<sup>12</sup></pre>
<pre><sup><strong>Note:</strong></sup></pre>
<pre><sup><strong>A new test file has been added that includes some tricky test cases on 29/09/14 and all submissions were rejudged.</strong></sup></pre>
<pre><sup><strong>Please don't ask the answers for additional test cases in the comments. Figure out yourself. </strong></sup></pre>