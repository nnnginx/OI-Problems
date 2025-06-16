<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">On the continent of Equestria, Dr. Whooves used to have it all. &nbsp;He owned a very successful transportation business which was connected to all the villages and towns of Equestria. &nbsp;However, when Discord took over Equestria, a lot of the ponies got confused. &nbsp;Even now, some of his workers are working at the wrong routes, and Dr. Whooves is pretty sure that his business is now fragmented, and that he isn't connected to all the villages of Equestria anymore.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Twilight Sparkle and her friends are here to help. &nbsp;Dr. Whooves knows that there is some minimum number of routes he'll need to add to make sure his business is reconnected. &nbsp;He asked Twilight Sparkle and her friends to find out how many different ways he can choose to add this minimum number of routes so that his business is connected to all the cities of Equestria. &nbsp;There might be a lot of ways, so the ponies have agreed upon giving the answer modulo 999,999,93</div>
<p><span style="font-size: small;"><span style="white-space: pre;"> </span>On the continent of Equestria, Dr. Whooves used to have it all. &nbsp;He owned a very successful transportation business which was connected to all the villages and towns of Equestria. &nbsp;However, when Discord took over Equestria, a lot of the ponies got confused. &nbsp;Even now, some of his workers are working at the wrong routes, and Dr. Whooves is pretty sure that his business is now fragmented, and that he isn't connected to all the villages of Equestria anymore.</span></p>
<p><span style="font-size: small;"><span style="white-space: pre;"> </span>Twilight Sparkle and her friends are here to help. &nbsp;Dr. Whooves knows that there is some minimum number of routes he'll need to add to make sure his business is reconnected. &nbsp;He asked Twilight Sparkle and her friends to find out how many different ways he can choose to add this minimum number of routes so that his business is connected to all the cities of Equestria. &nbsp;There might be a lot of ways, so the ponies have agreed upon giving the answer modulo 999,999,937.</span></p>
<p><span style="font-size: small;"><br></span></p>
<h3><span style="font-size: medium;">Input</span></h3>
<p><span><span style="font-size: small;">First is an integer T, the number of test cases, followed by T sets of data for each test case.</span></span></p>
<p><span style="font-size: small;">Each test case is in the following format:</span></p>
<p><span style="font-size: small;">It indicates that there are C cities, numbered 1 through C, and R routes, on a single line. &nbsp;After that follow R lines, each containing two city numbers Ai and Bi, indicating a bidirectional route between cities Ai and Bi.</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;">Test cases are not separated by blank lines, and the input ends with the last line of the final test case.</span></p>
<p>Constraints: 1 &lt;= C &lt;= 1000000, 0 &lt;= R &lt; min{C, 100000}</p>
<h3><span style="font-size: medium;">Output</span></h3>
<p><span style="font-size: small;">T lines, each containing the number of different ways Dr. Whooves can choose to add the minimum number of routes required to reconnect his business, modulo 999999937.</span></p>
<h3><span style="font-size: medium;">Example</span></h3>
<pre><strong>Input:</strong></pre>
<pre>4<br>4 0
3 1
1 2
5 4
1 2
2 3
3 4
2 5
7 6
2 3
3 4
2 4
5 6
6 7
7 5

<strong>Output:</strong>
16
2
1
63</pre>