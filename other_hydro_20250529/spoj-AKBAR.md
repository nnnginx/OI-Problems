<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">All of us are familiar with the reign of the great mughal ruler , Akbar. He was always concerned with the prosperity and safety of the people . Therefore to safeguard his kingdom (which consisted of N cities) he wanted to place secret soldiers all over his kingdom so as to protect the people . But since his kingdom is very large therefore he wanted to place as minimum of them as possible because the salary of these undercover soldiers was very high ,ie, in such a way that every city is protected by only one soldier .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp;As for these soldiers , they have varible strength .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The strength of a particular soldier is defined as the number of cities he can safeguard from a particular city along with that city.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Also the kingdom is connected with a network of secret two way roads for faster access only accessible to these soldiers. The length of any road on this network between any two cities is 1 kms .There are R such roads in the kingdom.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">He had given this task to birbal to place the soldiers . Birbal didn't wanted to be a fool in front of the king , therefore took the job and placed M soldiers all over the kingdom but he was not very good at mathematics . But since he is very intelligent he somehow places the guards all over the kingdom and now turns to you (who is a genius mathematician ;) ) to check whether his placements are good or not.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Your task is to check if all the placements of the soldiers are optimum or not.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">INPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The input consists of t test cases . Each test case then consists of 3 parts.The first line consists of N and R and M.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the next R lines consists of two numbers a and b denoting the two cities between which a road exists .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the next M lines consists of 2 numbers k and strength denoting the city number and the strength of that particular soldier respectively .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">=&gt; strength 0 means it will only guard the city on which it is present .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">=&gt; assume every city is accesible from every other city .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">CONSTRAINTS</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>t &lt;= 10;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>1 &lt;= N &lt;= 10^6;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>N-1 &lt;= R &lt;= min(10^9 , (N*(N-1))/2));</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>1 &lt;= k &lt;= N;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>0 &lt;= strength &lt;= 10^6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">OUTPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">print "Yes" if the soldiers are placed optimumly else print "No". (quotes are for clearity)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">SAMPLE INPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 2 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4 5 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">SAMPLE OUTPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">No</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Yes</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">WARNING ==&gt; Large input . Be careful with certain languages. Use scanf() for c/c++ ;</div>
<p>All of us are familiar with the reign of the great mughal ruler , Akbar. He was always concerned with the prosperity and safety of the people . Therefore to safeguard his kingdom (which consisted of N cities) he wanted to place secret soldiers all over his kingdom so as to protect the people . But since his kingdom is very large therefore he wanted to place them in such a way that every city is protected by <strong>one and only one</strong> soldier.According to Akbar , this is the optimum placement.</p>
<p>&nbsp;As for these soldiers they can protect multiple cities according to their strengths.</p>
<p>The strength of a particular soldier is defined as the maximum distance upto which a guard can protect a city from its base city(base city is the city assigned to the guard). If there are 3 cities C1, C2 and C3 such that C1 C2 and C2 C3 are connected respectively, if a soldier with strength 1 is placed at C2 then all the cities C1, C2 and C3 are protected by that soldier.</p>
<p>Also the kingdom is connected with a network of secret two way roads for faster access only accessible to these soldiers. The length of any road on this network between any two cities is 1 kms .There are R such roads in the kingdom.&nbsp;</p>
<p>He had given this task to birbal to place the soldiers . Birbal didn't wanted to be a fool in front of the king , therefore took the job and placed M soldiers all over the kingdom but he was not very good at mathematics . But since he is very intelligent he somehow places the guards all over the kingdom and now turns to you (who is a genius mathematician ;) ) to check whether his placements are good or not.</p>
<p>&nbsp;</p>
<p>Your task is to check if the placements of the soldiers are optimum or not.</p>
<p>&nbsp;</p>
<p><strong>INPUT</strong></p>
<p>&nbsp;</p>
<p>The input consists of <strong>T</strong> test cases . Each test case then consists of 3 parts.The first line consists of <strong>N,&nbsp;R </strong>and<strong> M</strong>.</p>
<p>the next <strong>R</strong> lines consists of two numbers <strong>A</strong>&nbsp;and <strong>B</strong>&nbsp;denoting the two cities between which a road exists .</p>
<p>the next <strong>M</strong> lines consists of 2 numbers, city number&nbsp;<strong>K</strong> and strength <strong>S</strong>&nbsp;of that particular soldier.</p>
<p>&nbsp;</p>
<p>=&gt; strength 0 means it will only guard the city on which it is present .</p>
<p>=&gt; assume every city is accesible from every other city .</p>
<p>&nbsp;</p>
<p><strong>CONSTRAINTS</strong></p>
<p>&nbsp;</p>
<p><span style="white-space: pre;"> <strong>T</strong></span>&nbsp;&lt;= 10;</p>
<p><span style="white-space: pre;"> </span>1 &lt;= <strong>N</strong> &lt;= 10^6;</p>
<p><span style="white-space: pre;"> </span><strong>N&nbsp;</strong>-1 &lt;= <strong>R</strong> &lt;= <strong>min</strong>( 10^7 , (&nbsp;<strong>N&nbsp;</strong>* (<strong>N&nbsp;</strong>- 1) ) / 2) );</p>
<p><span style="white-space: pre;"> </span>1 &lt;= <strong>K</strong> &lt;= <strong>N</strong>;</p>
<p><span style="white-space: pre;"> </span>0 &lt;= <strong>S</strong> &lt;= 10^6</p>
<p>&nbsp;</p>
<p><strong>OUTPUT</strong></p>
<p>&nbsp;</p>
<p>print "Yes" if the soldiers are placed optimumly else print "No". (quotes are for clarity)</p>
<p>&nbsp;</p>
<p><strong>SAMPLE INPUT</strong></p>
<p>&nbsp;</p>
<p>2</p>
<p>3 2 2</p>
<p>1 2</p>
<p>2 3</p>
<p>1 2</p>
<p>2 0</p>
<p>4 5 2</p>
<p>1 4</p>
<p>1 2</p>
<p>1 3</p>
<p>4 2</p>
<p>3 4</p>
<p>2 1</p>
<p>3 0</p>
<p>&nbsp;</p>
<p><strong>SAMPLE OUTPUT</strong></p>
<p>&nbsp;</p>
<p>No</p>
<p>Yes</p>
<p>&nbsp;</p>
<p><strong>WARNING</strong> ==&gt; Large input.</p>
<p>&nbsp;</p>