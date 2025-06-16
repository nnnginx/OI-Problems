<p><em>[The original version of this problem (in Spanish) can be found at&nbsp;<a href="http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf</a>]</em></p>
<p>&nbsp;</p>
<p>Every year the kingdoms of Cubiconia, Quadradonia and Nlogonia&nbsp;organize a ball to commemorate the end of the war that ravaged&nbsp;the region for many years. A certain number of noblemen of each&nbsp;kingdom is invited to participate in this event, and it is&nbsp;expected that every pair of guests coming from different&nbsp;kingdoms will dance together exactly once. That is, each of the&nbsp;guests from Cubiconia shall dance once with every guest from&nbsp;Quadradonia and Nlogonia; in turn, each of the guests from&nbsp;Quadradonia shall also dance once with every guest from&nbsp;Nlogonia. However, guests coming from the same kingdom are not&nbsp;allowed to dance with one another.</p>
<p>To help organize the ball, the total number of dances that will&nbsp;take place is determined beforehand, so that care must be taken&nbsp;when choosing the number of noblemen that shall be invited from&nbsp;each kingdom. For example, if it is decided that the ball must&nbsp;have <strong>N = 20</strong> dances, one possibility is to invite <strong>6</strong> noblemen&nbsp;from Cubiconia, <strong>2</strong> from Quadradonia and <strong>1</strong> from Nlogonia, which&nbsp;can be represented by the expression <strong>(6, 2, 1)</strong>. This is a valid&nbsp;option because the total number of dances would then be <strong>6*2 +&nbsp;6*1 + 2*1 = 20</strong>.</p>
<p>Traditions whose origins nobody can now remember indicate that&nbsp;the number of invited noblemen from Cubiconia must be greater&nbsp;or equal to the number of those coming from Quadradonia, and at&nbsp;the same time the number of invited noblemen from Quadradonia&nbsp;must be greater or equal to those coming from Nlogonia. Thus,&nbsp;for <strong>N = 20</strong> dances there are exactly <strong>5</strong> possible ways to choose&nbsp;the number of guests from each kingdom, namely <strong>(5, 4, 0)</strong>, <strong>(4,&nbsp;2, 2)</strong>, <strong>(10, 2, 0)</strong> and&nbsp;<strong>(20, 1, 0)</strong> as well as the aforementioned <strong>(6,&nbsp;2, 1)</strong>.</p>
<p>With so many restrictions, the organizing committee has&nbsp;problems finding the ideal way to choose the number of guests&nbsp;from each kingdom. Your task is to help this committee by&nbsp;counting the different ways in which the number of guests can&nbsp;be chosen for a ball with <strong>N</strong> dances. Two of these ways are&nbsp;considered different if they differ in the number of invited&nbsp;noblemen from at least on of the three kingdoms.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Each test case is described using a single line, containing an&nbsp;integer <strong>N</strong> representing the total number of dances that the ball&nbsp;must have (<strong>1 ��&nbsp;N ��&nbsp;10<sup>4</sup></strong>). The end of the input is signalled&nbsp;by a line containing the number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print a single line containing the number&nbsp;of different ways in which the number of guests from each&nbsp;kingdom can be chosen in order to have a ball where there are&nbsp;exactly <strong>N</strong> dances, with all the restrictions mentioned in the&nbsp;problem statement.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">20
1
9747
-1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">5
1
57</span></pre>