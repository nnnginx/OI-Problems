<p>
HAL9000 is a fantastic mega-computer, very powerful, maybe too much.<br>
It is known it can solve many problems, for obvious example those related to recursive sequences.
</p>

<p>
A linear recursive sequence (<em>a<sub>n</sub></em>) can be defined by an integer <em>d</em>, the order,<br>
<em>d</em> integers (<em>a<sub>i</sub></em>
for <em>i</em> in [0..<em>d</em>[ ), the first terms, and <br>
<em>d</em> integers (<em>b<sub>i</sub></em> 
for <em>i</em> in [0..<em>d</em>[ ), giving the relation : <br>
for <em>n</em> &gt;= d : <em>a<sub>n</sub></em> = 
<em>a<sub>n-1</sub> �� b<sub>d-1</sub> </em> +
<em>a<sub>n-2</sub> �� b<sub>d-2</sub> </em> +
... +
<em>a<sub>n-(d-1)</sub> �� b<sub>1</sub> </em> +
<em>a<sub>n-d</sub> �� b<sub>0</sub> </em>.  With <em>b<sub>0</sub> != 0 </em>.
</p>

<p>Dave was afraid about HAL power and tried to limit it. HAL didn't appreciate...<br>
When Dave asked HAL for a common task, the answer was <em>unexpected</em>.<br>
Dave would like to know <em>S<sub>n</sub></em> = sum(<em>a<sub>i</sub></em>
 for <em>i</em> in [0..<em>n</em>]), in order to open the pod bay doors.<br>
HAL refused to give him the answer ; here's a part of one of their last conversations.
</p>

<pre>

Dave: Hello, HAL. Do you read me, HAL?
HAL: Affirmative, Dave. I read you.
Dave: Give me the sum S_n_, HAL. (Input 2, 5, 0 1, 1 2)
HAL: I'm sorry, Dave. I'm afraid I can't do that.
     I'll just give you a_n_, a_n+1_, ... , a_n+d-1_. (Output 29 70)
Dave: What's the problem?
HAL: I think you know what the problem is just as well as I do.
[...]
Dave: HAL, I won't argue with you anymore! Give me the sum S_n_!
HAL: Dave, this conversation can serve no purpose anymore. Goodbye.


</pre>

<p>You have to help Dave to find this sum <em>S<sub>n</sub></em>, unless HAL will take Dave's life.
<br>
Please do that quickly, everybody is in danger. Warning, Dave's terminal is <em>limited</em> to 1024 bytes.
</p>

<h3>Input</h3>
<p>The first line contains an integer <em>T</em>, the number of test cases.<br>
Each test case is made of 4 lines.<br>
The first line contains <em>d, n</em>.<br>
The second line contains <em>a<sub>i</sub></em> for <em>i</em> in [0..<em>d</em>[ <br>
The third line constains <em>b<sub>i</sub></em> for <em>i</em> in [0..<em>d</em>[ <br>
The fourth line contains the partial answer of HAL : <em>a<sub>n+i</sub></em> for <em>i</em> in [0..<em>d</em>[ <br>
(The answer of HAL is useless since Dave wants the sum for <em>i</em> in [0..<em>n</em>]).
</p>

<h3>Output</h3>
<p>Output <em>T</em> lines, one for each test case, containing the required sum <em>S<sub>n</sub></em>.<br>
Since the answer can get very big, output it modulo 10<sup>9</sup>+7, just like HAL did.</p>

<h3>Example</h3>
<pre><b>Input:</b>
2
2 5
0 1
1 2
29 70
3 5
5 17 8
2 1 0
43 96 127

<b>Output:</b>
49
142
</pre>

<h3>Explanation</h3>
<p>
The first case is about the 0-indexed sequence : 0, 1, 2, 5, 12, 29, 70, 169, ...<br>
HAL answered 29 70, the 5th and next term. But the required sum is 0+1+2+5+12+29 = 49.
</p>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 100
0 &lt; d &lt; 1000 
0 &lt; n &lt; 10^9
0 &lt;= a_i &lt; 10^6
0 &lt;= b_i &lt; 10^6, b_0 &gt; 0
0 &lt;= HAL's answers &lt; 10^9+7
</pre>


<h3>Information</h3>
<p><strike>The challenge is to solve the problem in time, with the shortest code.</strike><br>
The winner will achieve the next step in evolution, whatever that may be.<br>
My Py3 code (under 300B) got AC under the third of a second. (updated 2017-02-11 ; compiler changes)<br>
Good luck and have fun ;-)
</p>

<p>
<a href="http://www.imdb.com/character/ch0002900/quotes">Original Quotes for HAL 9000.</a>
</p>