<p>Few years back IUT(International University Of Technology) authority decided to increase the number of students. As more students are getting admitted every year but the number of classroom didn't increase, the classrooms became overpopulated. As people are complaining about this, and making new classrooms is not possible in next few years one of the very intelligent person of the authority gave an idea to tackle this situation. It is that, they will not increase the classrooms rather they will distribute the classes into rooms such a way that it doesn't look like overpopulated although all the students come out of the class at the same time. So, It'll create an illution amongst the visitor and they will think IUT is great as before.</p>
<p>The distribution process&nbsp; is that for every class this class will either contain more students than all the adjacent classes or contain less students than the adjacent classes. All the classes are situated in a line , so each class has two adjacent classroom except the 1st and the last classroom.</p>
<p>suppose there are n classroom and the number of students of that classrooms are&nbsp; &nbsp;<span style="font-size: x-small;"><span style="color: #4a4a4a; box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>1</sub></span><span style="color: #4a4a4a;">&nbsp;,&nbsp;</span><span style="color: #4a4a4a; box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>2</sub></span><span style="color: #4a4a4a;">&nbsp;,&nbsp;</span><span style="color: #4a4a4a; box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>3</sub></span><span style="color: #4a4a4a;">&nbsp;,&nbsp;</span><span style="color: #4a4a4a; box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>4</sub></span><span style="color: #4a4a4a;">&nbsp;.......... ...&nbsp;</span><span style="color: #4a4a4a; box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>N</sub></span></span></p>
<p><span style="color: #4a4a4a;"><span style="font-size: xx-small;">You'll have to distribute the classes as</span></span></p>
<ul style="box-sizing: border-box; margin: 0px 0px 20px 25px; padding: 0px; font-variant-numeric: normal; font-variant-east-asian: normal; font-stretch: normal; font-size: 15px; line-height: 1.7; font-family: Helvetica, sans-serif; list-style-position: outside; color: #4a4a4a;">
<li style="box-sizing: border-box; margin: 0px; padding: 0px;"><span style="font-size: x-small;"><span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>1</sub></span>&nbsp;&gt;&nbsp;<span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>2</sub></span>&nbsp;&lt;&nbsp;<span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>3</sub></span>&nbsp;&gt;&nbsp;<span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>4</sub></span>&nbsp;&lt; ...&nbsp;<span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>N or</sub></span></span></li>
<li style="box-sizing: border-box; margin: 0px; padding: 0px;"><span style="font-size: x-small;"><span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>1</sub></span>&nbsp;&lt;&nbsp;<span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>2</sub></span>&nbsp;&gt;&nbsp;<span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>3</sub></span>&nbsp;&lt;&nbsp;<span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>4</sub></span>&nbsp;&gt; ...&nbsp;<span style="box-sizing: border-box; font-weight: 700; line-height: inherit;">a<sub>N</sub></span></span></li>
</ul>
<p>However you can only do one type of operation. You can swap the classrooms at position i and n-i+1.</p>
<p>You'll have to determine the mimimum number of operations to distrubute the classrooms and make IUT great again. If it's impossible print -1</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line of the input contains t, number of testcases,</p>
<p>Then each testcase takes a integer n, number of rooms and then n integers the population of n'th class.</p>
<p>1&lt;t&lt;10</p>
<p>0&lt;n&lt;10<sup>5</sup></p>
<p>0&lt;a<sub>i</sub>&lt;10<sup>9</sup></p>
<h3>Output</h3>
<p>For each testcase on separate line print the minimum number of operations or -1 if not possible</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>2</pre>
<pre>6</pre>
<pre>1 2 3 4 5 6</pre>
<pre>5</pre>
<pre>5 2 4 3 5</pre>
<pre><strong>Output:</strong></pre>
<pre>1</pre>
<pre>0</pre>