<p><span style="font-weight: bold;"><span style="font-size: small;"><span class="GingerNoCheckStart">&nbsp;</span>Problem Statement:</span></span></p>
<p><span style="font-size: small;">The Maya is a Mesoamerican civilization noted for its&nbsp;art, architecture, mathematics and astronomical systems. In the recent past their calendar system has been quite in the news because of the misinterpretation of their Long count calendar, which gave way for a popular belief that a cataclysm will take place on December 21, 2012.&nbsp;Many speculated it will mark the end of human civilization!</span></p>
<p><span style="font-size: small;">But we now know it did not happen as we are still alive! Note this date, it falls on a Friday.Since human civilization may have ended on that day, we will call every Friday the 21st as a <em>vulnerable</em> day. Similarly we define a <em>safe</em> day which is not a vulnerable day. Your task is given two years M and N, you need to find how many safe days are there between any given years M and N (inclusive).</span></p>
<p><span style="font-size: small;">To honor the Mayan civilization you should write the total number of safe days in Mayan Long Count notation. The Long Count calendar identifies a date by counting the number of days from the Mayan creation date. But instead of using a base-10 scheme like Western numbering, the Long Count days were tallied in a modified base-20 scheme. As a matter of fact December 21, 2012 is simply the day that the calendar will go to the next B'ak'tun. You do not need to bother about creation date but simply represent your answer in Long Count notation. See the below example and table for clarification:</span></p>
<p><span style="font-size: small;"><br></span></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="229" valign="top">
<p align="center"><strong><span style="font-size: small;">Days</span></strong></p>
</td>
<td width="234" valign="top">
<p align="center"><strong><span style="font-size: small;">Place</span></strong></p>
</td>
<td width="210" valign="top">
<p align="center"><strong><span style="font-size: small;">Long Count unit</span></strong></p>
</td>
</tr>
<tr>
<td width="229" valign="top">
<p><span style="font-size: small;">1</span></p>
</td>
<td width="234" valign="top">
<p><span style="font-size: small;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 0</span></p>
</td>
<td width="210" valign="top">
<p><span style="font-size: small;">1 K'in</span></p>
</td>
</tr>
<tr>
<td width="229" valign="top">
<p><span style="font-size: small;">20</span></p>
</td>
<td width="234" valign="top">
<p><span style="font-size: small;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1</span></p>
</td>
<td width="210" valign="top">
<p><strong><span style="font-size: small;">1 Winal</span></strong></p>
</td>
</tr>
<tr>
<td width="229" valign="top">
<p><span style="font-size: small;">360</span></p>
</td>
<td width="234" valign="top">
<p><span style="font-size: small;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2</span></p>
</td>
<td width="210" valign="top">
<p><span style="font-size: small;">1 Tun</span></p>
</td>
</tr>
<tr>
<td width="229" valign="top">
<p><span style="font-size: small;">7,200</span></p>
</td>
<td width="234" valign="top">
<p><span style="font-size: small;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3</span></p>
</td>
<td width="210" valign="top">
<p><span style="font-size: small;">1 K'atun</span></p>
</td>
</tr>
<tr>
<td width="229" valign="top">
<p><span style="font-size: small;">144,000</span></p>
</td>
<td width="234" valign="top">
<p><span style="font-size: small;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4</span></p>
</td>
<td width="210" valign="top">
<p><span style="font-size: small;">1 B'ak'tun</span></p>
</td>
</tr>
</tbody>
</table>
<p><strong><span style="font-size: small;">Table of Long Count units</span></strong></p>
<p><span style="font-size: small;">Check the full list here: <a href="http://en.wikipedia.org/wiki/Maya_calendar">http://en.wikipedia.org/wiki/Maya_calendar</a> (not needed for this problem).</span></p>
<p><span style="font-size: small;"><strong>Conversion</strong>:</span></p>
<p><span style="font-size: small;">For this problem you can consider numbers in the Long Count to be represented in base 20 except for the <strong>Winal</strong> place which is to be taken in base 18. Below example will clarify how to convert your answer into Long Count Notation.</span></p>
<p><span style="font-size: small;">For instance, if safe days comes out to be 1454 your output must be:&nbsp; "0.0.4.0.14" (without quotes).&nbsp;&nbsp;&nbsp; (1*14 + 20*0 + 360*4 + 7200*0 + 144000*0 = 1454)</span></p>
<p><span style="font-size: small;">For 360 output must be "0.0.1.0.0"(without quotes).</span></p>
<p><span style="font-size: small;">For 20 output must be ��0.0.0.1.0�� (without quotes).</span></p>
<p><span style="font-size: small;">As you can see all the places are in base 10 except the 1<sup>st</sup> place which is base 18.</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>Input Specification</strong>: First line of input contains 0&lt;T&lt;500, number of test cases on which your program will run. Followed by two integers M and N where &nbsp;1901&lt;=M, N&lt;=2300, where M&lt;=N, if M=N you need to tell for that particular year only.</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>Output Specification</strong>: For every test case output: A single line containing the number of safe days between the year M and N(inclusive) in Long count notation explained above. It is guaranteed that the number of safe days could always be represented up to fourth place (B'ak'tun place) in the above given notation.</span></p>
<p><span style="font-size: small;">"a.b.c.d.e" (without quotes) where&nbsp;&nbsp;&nbsp; 0&lt;= a, b, c, e &lt;20, 0&lt;=d&lt;18.</span></p>
<p><span style="font-size: small;"><strong>Facts</strong>:</span></p>
<ol>
<li><span style="font-size: small;">Jan 1, 1901 was Tuesday.</span></li>
<li><span style="font-size: small;">All calculations must be done following Gregorian calendar which is the current standard calendar in the world including ours.</span></li>
<li><span style="font-size: small;">If you don't know how to calculate leap year see this link: &lt;<a href="http://en.wikipedia.org/wiki/Leap_year">http://en.wikipedia.org/wiki/Leap_year</a>&gt;</span></li>
</ol>
<p><strong><span style="font-size: small;">Sample Test cases:</span></strong></p>
<p><strong><span style="font-size: small;">Input:</span></strong></p>
<p><span style="font-size: small;">3</span></p>
<p><span style="font-size: small;">2011 2012</span></p>
<p><span style="font-size: small;">2012 2012</span></p>
<p><span style="font-size: small;">2000 2020</span></p>
<p><strong><span style="font-size: small;">Output:</span></strong></p>
<p><span style="font-size: small;">0.0.2.0.7</span></p>
<p><span style="font-size: small;">0.0.1.0.4</span></p>
<p><span style="font-size: small;">0.1.1.3.14</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><strong><span style="font-size: small;">Explanation: </span></strong></p>
<p><span style="font-size: small;">For case 1: there are 727 safe days which can be represented as 0.0.2.0.7</span></p>
<p><span style="font-size: small;">There are 4 vulnerable days between: January 2011 to December 2012.</span></p>
<p><span style="font-size: small;">These are: 21<sup>st</sup> January 2011, 21<sup>st</sup> October 2011, 21<sup>st</sup> September 2012 and 21st December 2012.</span></p>
<p><span style="font-size: small;">Total number of days between: January 2011 to December 2012 are 731.</span></p>
<p><span style="font-size: small;">Therefore the number of safe days are 731-4 = 727.</span></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><span class="GingerNoCheckEnd">&nbsp;</span></p>