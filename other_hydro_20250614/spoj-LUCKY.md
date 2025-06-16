<p><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">John has recently arrived in Romania for the South Eastern European Regional competitions. John has never been to Romania before so Romanians decided to organize sightseeing tour for him. This tour will include several Romanian cities and none of them will be visited more than once. John will start in one city and will visit some other cities according to a guide tour. At the end of the tour John will return to the starting point.</span></p>
<p><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;"><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">There are N cities numbered from 1 to N and M two-way roads in the country. Each road connects two different cities. Consider a sightseeing tour for John c<sub>1</sub>,c<sub>2</sub>,...,c<sub>n</sub>, where each ci denotes a city in Romania. Then all c<sub>i</sub> must be distinct, c<sub>i</sub> and c<sub>i+1</sub>&nbsp;must be connected by a road, where i=1,2,...,n-1, c<sub>n</sub> and c<sub>1</sub> must be connected by a road as well.&nbsp;</span></span></p>
<p><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;"><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">Being a odd person John would like to visit an odd number of cities. The organizers have drawn the plan of all possible tours with an odd number of cities.&nbsp;</span></span></p>
<p><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;"><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">Residents of the cities would like John to visit them. So if there is at least one tour passing through some city than this city is called lucky. Your task is to calculate the number of lucky cities in Romania.</span></span></p>
<h3>Input</h3>
<p><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">The first line of input contains a single integer T �C a number of test cases. Every test case starts with a line containing two integers separated by a single space �C N and M. Each of the next M lines will contain two integers a<sub>i</sub> and b<sub>i</sub> separated by a single space �C the labels of cities that i-th road connects.</span></p>
<h3>Output</h3>
<p><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">Output should contain T lines �C answers for each of the test cases.</span></p>
<h3>Constraints</h3>
<p><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">1 �� T �� 77,&nbsp;</span><br style="font-family: 'Times New Roman', Times, serif; font-size: 16px;"><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">0 �� N, M �� 100000 (10<sup>5</sup></span><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">),&nbsp;</span><br style="font-family: 'Times New Roman', Times, serif; font-size: 16px;"><span style="font-family: 'Times New Roman', Times, serif; font-size: 16px;">1 �� a<sub>i</sub> &lt; b<sub>i</sub> �� N</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: medium;">1 
7 7 
1 5 
3 5 
3 7 
1 7 
6 7 
4 7 
4 6</pre>
<strong>Output:</strong>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: medium;">3</pre>
</pre>
<pre><em><span style="font-size: small;"><strong>PS:</strong> If you like this problem, also see problem BUSINESS</span></em></pre>