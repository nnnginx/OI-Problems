<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">"I read somewhere that everybody on this planet is separated by only six other people. Six</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">degrees of separation between us and everyone else on this planet. The President of the United</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">States, a gondolier in Venice, just ll in the names. I nd it A) extremely comforting that</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">we're so close, and B) like Chinese water torture that we're so close because you have to nd</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the right six people to make the right connection... I am bound to everyone on this planet by</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">a trail of six people." { Ouisa Kitteridge, "Six Degrees of Separation"</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Is widely know that one is separated from everyone in the world in no more than 6 degrees of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">separation. A degree of separation is dened by the minimum numbers of connections you need</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">to make to contact someone else. For instance, if you know personally another person, then</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">you are separated by one degree. If you know somebody through some friend but not directly</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(a friend of a friend), then you are separated by two degrees, and so on.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Nevertheless, young Kevin Smith is not convinced about this theory and wants to probe it false.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">To achieve this, he has hacked the Hi6! social network and requested you to help him knock</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">down the theory of six degrees of separation</div>
<p style="text-align: justify;">"I read somewhere that everybody on this planet is separated by only six other people. Six&nbsp;degrees of separation between us and everyone else on this planet. The President of the United&nbsp;States, a gondolier in Venice, just ll in the names. I find it A) extremely comforting that&nbsp;we're so close, and B) like Chinese water torture that we're so close because you have to find&nbsp;the right six people to make the right connection... I am bound to everyone on this planet by&nbsp;a trail of six people." - Ouisa Kitteridge, "Six Degrees of Separation"</p>
<p style="text-align: justify;">Is widely know that one is separated from everyone in the world in no more than 6 degrees of&nbsp;separation. A degree of separation is defined by the minimum numbers of connections you need&nbsp;to make to contact someone else. For instance, if you know personally another person, then&nbsp;you are separated by one degree. If you know somebody through some friend but not directly&nbsp;(a friend of a friend), then you are separated by two degrees, and so on.</p>
<p>Nevertheless, young Kevin Smith is not convinced about this theory and wants to probe it false.&nbsp;To achieve this, he has hacked the Hi6! social network and requested you to help him knock&nbsp;down the theory of six degrees of separation.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line contains an integer T, which specifies the number of test cases. Then, T test case&nbsp;descriptions will follow.&nbsp;Each test case will start with a line with one positive integer, N meaning the number of&nbsp;connections. The next N lines will contain the following pattern:</p>
<p>&lt;name_1&gt; &lt;name_2&gt; &lt;D&gt;</p>
<p>meaning that person "&lt;name_1&gt;" is connected with the person "&lt;name_2&gt;" by making D connections and viceversa. Note that both persons can know each other by a lower degree of&nbsp;separation using other connections.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each input case you must print the string "Case #i: ", where i is the test case number,&nbsp;starting from 1, following by the maximum degree of separation between the specified people.&nbsp;If there is someone that cannot connect to another person, print "INFINITE" instead.</p>
<p>&nbsp;</p>
<h3>Constraints</h3>
<ul>
<li>All names will be non-empty strings composed only by lowercase characters.</li>
<li>All names will have between 1 and 10 characters, inclusive.</li>
<li>"&lt;name_1&gt;" will be different than "&lt;name_2&gt;" for all connections.</li>
<li>There will be no pair of connections between the same pair of persons.</li>
<li>D will be an integer between 1 and 1000, inclusive, for all connections.</li>
<li>T will be between 1 and 100, inclusive.</li>
<li>N will be between 1 and 10^5, inclusive.</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br></pre>
<pre>3<br>2<br>john judy 1<br>mary peter 1<br>3<br>john judy 7<br>john peter 2<br>judy peter 2<br>7<br>john judy 3<br>katie peter 4<br>john peter 2<br>judy mary 1<br>peter mary 2<br>john katie 1<br>katie mary 1<br><br><br><strong>Output:</strong><br></pre>
<pre>Case #1: INFINITE<br>Case #2: 4<br>Case #3: 3<br></pre>