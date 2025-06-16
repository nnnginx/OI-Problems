<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Organizing CS contests didn't prove very lucrative for Mirko, so he has opened an ice cream and pastry&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">shop. The business was flourishing until, one day, the European Union health inspection decided to&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">pay him a visit.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A new directive specifies M banned ingredients which cannot appear in food even in trace amounts.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each ingredient has a serial number consisting of digits 0 through 9. The declaration on each food&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">package lists all the serial numbers of ingredients contained in the respective food item.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Mirko must check whether any of his products has a banned ingredient serial number listed on its&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">declaration. However, Mirko, being inept and reckless as always, decided to concatenate all the serial&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">numbers into one long number with length N believing that it will make his job easier. He has&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">borrowed a robot from his friend Slavko. The robot is programmed to check whether a serial number&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A contains another serial number B as a substring. Let us denote the length of B by L. The robot&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">carries out search as follows:&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• First, it compares the segment of A from position 1 to position L, digit by digit, with the digits&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">in B. Comparison is stopped when a differing digit is found or when the segments are&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">determined to be equal. If the segments are equal, the search is stopped and the match&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">reported.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• If the segments are not equal, the procedure above is repeated with the segment from 2 to L+1.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">If those segments aren't equal either, the search continues with segments 3 to L+2, 4 to L+3&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">etc.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• If the robot doesn't have a sufficient number of digits to obtain a full segment of length L (for&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">example, starting at character 5 in a serial number with length 8, a segment with length 6 is&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">needed), it will pad the number with '#' signs. For example, the segment of "563232" from&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">position 4 to position 10 is "232####".&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• If the robot reaches the end of the serial number (having tried out all N segments) without&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">having found B, the absence of match is reported.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The robot takes one second for each comparison between two digits, and Slavko charges Mirko one&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">dollar per second for using the robot.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Help Mirko determine how much money he'll have to pay Slavko for pattern matching!&nbsp;</div>
<p>Organizing CS contests didn't prove very lucrative for Mirko, so he has opened an ice cream and pastry shop. The business was flourishing until, one day, the European Union health inspection decided to pay him a visit. A new directive specifies M banned ingredients which cannot appear in food even in trace amounts. Each ingredient has a serial number consisting of digits 0 through 9. The declaration on each food package lists all the serial numbers of ingredients contained in the respective food item. Mirko must check whether any of his products has a banned ingredient serial number listed on its declaration. However, Mirko, being inept and reckless as always, decided to concatenate all the serial numbers into one long number with length N believing that it will make his job easier. He has borrowed a robot from his friend Slavko. The robot is programmed to check whether a serial number A contains another serial number B as a substring. Let us denote the length of B by L. The robot carries out search as follows:</p>
<p>• First, it compares the segment of A from position 1 to position L, digit by digit, with the digits in B. Comparison is stopped when a differing digit is found or when the segments are determined to be equal. If the segments are equal, the search is stopped and the match reported.&nbsp;</p>
<p>• If the segments are not equal, the procedure above is repeated with the segment from 2 to L+1. If those segments aren't equal either, the search continues with segments 3 to L+2, 4 to L+3 etc.&nbsp;</p>
<p>• If the robot doesn't have a sufficient number of digits to obtain a full segment of length L (for example, starting at character 5 in a serial number with length 8, a segment with length 6 is needed), it will pad the number with '#' signs. For example, the segment of "563232" from position 4 to position 10 is "232####".&nbsp;</p>
<p>• If the robot reaches the end of the serial number (having tried out all N segments) without having found B, the absence of match is reported.&nbsp;</p>
<p>&nbsp;</p>
<p>The robot takes one second for each comparison between two digits, and Slavko charges Mirko one dollar per second for using the robot. Help Mirko determine how much money he'll have to pay Slavko for pattern matching!&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of input contains the positive integer N (1 ≤ N ≤ 100 000), the length of the long serial&nbsp;</p>
<p>number.&nbsp;</p>
<p>The second line of input contains N digits from 0 to 9, the long serial number.&nbsp;</p>
<p>The third line of input contains the positive integer M (1 ≤ M ≤ 50 000), the number of banned&nbsp;</p>
<p>ingeredients.&nbsp;</p>
<p>Each of the following M rows contains a single banned serial number,&nbsp;</p>
<p>A banned serial number will not exceed 100 000 digits in length.&nbsp;</p>
<p>The total length of all banned serial numbers will not exceed 3 000 000 digits.&nbsp;</p>
<h3>Output</h3>
<p>Output M integers, one per line. Line i must contain the dollar amount that Mirko needs to pay Slavko&nbsp;</p>
<p>for the search for ingredient serial number i.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7 
1090901 
4 
87650 
0901 
109 
090 

<strong>Output:</strong>
7 
10 
3 
4 <span style="white-space: normal;">
</span></pre>
<pre><strong><br></strong></pre>
<pre><strong>Input:</strong>
10 
5821052680 
4 
210526 
2105 
582 
105268 

<strong>Output:</strong>
8 
6 
3 
9&nbsp;</pre>
<pre><strong><br></strong></pre>
<pre><strong>Input:</strong>
3 
001 
1 
11 

<strong>Output:</strong>
</pre>
<pre>4 </pre>