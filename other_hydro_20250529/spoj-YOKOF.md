<p>Starting with&nbsp;<span><em>x</em></span> and repeatedly multiplying by&nbsp;<span><em>x</em></span>, we can compute&nbsp;<span><em>x</em><sup>31</sup></span> with thirty multiplications:</p>
<blockquote><span><em>x</em><sup>2</sup> = <em>x</em> <tt>*</tt> <em>x</em></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>3</sup> = <em>x</em><sup>2</sup> <tt>*</tt> <em>x</em></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>4</sup> = <em>x</em><sup>3</sup> <tt>*</tt> <em>x</em></span>,&nbsp;&nbsp;&nbsp;&nbsp; <span>... &nbsp;,</span>&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>31</sup> = <em>x</em><sup>30</sup> <tt>*</tt> <em>x</em></span>.</blockquote>
<p>The operation of squaring can appreciably shorten the sequence of multiplications. The following is a way to compute&nbsp;<span><em>x</em><sup>31</sup></span> with eight multiplications:</p>
<blockquote><span><em>x</em><sup>2</sup> = <em>x</em> </span><span><tt>*</tt></span><span> <em>x</em></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>3</sup> = <em>x</em><sup>2</sup> </span><span><tt>*</tt></span><span><tt></tt> <em>x</em></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>6</sup> = <em>x</em><sup>3</sup> </span><span><tt>*</tt></span><span><tt></tt> <em>x</em><sup>3</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>7</sup> = <em>x</em><sup>6</sup> </span><span><tt>*</tt></span><span><tt></tt> <em>x</em></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>14</sup> = <em>x</em><sup>7</sup> </span><span><tt>*</tt></span><span> <em>x</em><sup>7</sup></span>, <br> <span><em>x</em><sup>15</sup> = <em>x</em><sup>14</sup> </span><span><tt>*</tt></span><span> <em>x</em></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>30</sup> = <em>x</em><sup>15</sup> </span><span><tt>*</tt></span><span> <em>x</em><sup>15</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>31</sup> = <em>x</em><sup>30</sup> </span><span><tt>*</tt></span><span> <em>x</em></span>.</blockquote>
<p>This is not the shortest sequence of multiplications to compute&nbsp;<span><em>x</em><sup>31</sup></span>. There are many ways with only seven multiplications. The following is one of them:</p>
<blockquote><span><em>x</em><sup>2</sup> = <em>x</em> </span><span><tt>*</tt></span><span> <em>x</em></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>4</sup> = <em>x</em><sup>2</sup> </span><span><tt>*</tt></span><span> <em>x</em><sup>2</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>8</sup> = <em>x</em><sup>4</sup> </span><span><tt>*</tt></span><span> <em>x</em><sup>4</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>10</sup> = <em>x</em><sup>8</sup> </span><span><tt>*</tt></span><span> <em>x</em><sup>2</sup></span>, <br> <span><em>x</em><sup>20</sup> = <em>x</em><sup>10</sup> </span><span><tt>*</tt></span><span> <em>x</em><sup>10</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>30</sup> = <em>x</em><sup>20</sup> </span><span><tt>*</tt></span><span> <em>x</em><sup>10</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>31</sup> = <em>x</em><sup>30</sup> </span><span><tt>*</tt></span><span> <em>x</em></span>.</blockquote>
<p>There however is no way to compute&nbsp;<span><em>x</em><sup>31</sup></span> with fewer multiplications. Thus this is one of the most efficient ways to compute&nbsp;<span><em>x</em><sup>31</sup></span> only by multiplications.</p>
<p>If division is also available, we can find a shorter sequence of operations. It is possible to compute&nbsp;<span><em>x</em><sup>31</sup></span> with six operations (five multiplications and one division):</p>
<blockquote><span><em>x</em><sup>2</sup> = <em>x</em> </span><span><tt>*</tt></span><span> <em>x</em></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>4</sup> = <em>x</em><sup>2</sup> </span><span><tt>*</tt></span><span><tt></tt> <em>x</em><sup>2</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>8</sup> = <em>x</em><sup>4</sup> </span><span><tt>*</tt></span><span><tt></tt> <em>x</em><sup>4</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>16</sup> = <em>x</em><sup>8</sup> </span><span><tt>*</tt></span><span><tt></tt> <em>x</em><sup>8</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>32</sup> = <em>x</em><sup>16</sup> </span><span><tt>*</tt></span><span> <em>x</em><sup>16</sup></span>,&nbsp;&nbsp;&nbsp;&nbsp;  <span><em>x</em><sup>31</sup> = <em>x</em><sup>32</sup> ¡Â <em>x</em></span>.</blockquote>
<p>This is one of the most efficient ways to compute&nbsp;<span><em>x</em><sup>31</sup></span> if a division is as fast as a multiplication.</p>
<p>Your mission is to write a program to find the least number of operations to compute <span><em>x</em><sup>n</sup></span> by multiplication and division starting with&nbsp;<span><em>x</em></span> for the given positive integer&nbsp;<span><em>n</em></span>. Products and quotients appearing in the sequence of operations should be <span><em>x</em></span> to a positive integer's power. In other words, <span><em>x</em><sup>-3</sup></span>, for example, should never appear.</p>
<h3>Input</h3>
<p>The input is a sequence of one or more lines each containing a single integer&nbsp;<span><em>n</em></span>. <span><em>n</em></span> is positive and less than or equal to 1000. The end of the input is indicated by a zero.</p>
<h3>Output</h3>
<p>Your program should print the least total number of multiplications and divisions required to compute <span><em>x</em><sup>n</sup></span> starting with&nbsp;<span><em>x</em></span> for the integer&nbsp;<span><em>n</em></span>.  The numbers should be written each in a separate line without any superfluous characters such as leading or trailing spaces.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
31
70
91
473
512
811
953
0

<strong>Output:</strong>&nbsp;
0
6
8
9
11
9
13
12</pre>