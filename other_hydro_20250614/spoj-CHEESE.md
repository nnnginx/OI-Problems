<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Nlogonian people is very excited about the event that will occur in the next year: the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Cheese-rolling World Cup Nlogonia 2013! The event is organized by the Modern Cheeserolling Association (MCA or ACM, as spelled in Nlogonish) every four years, and this will be</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">the ﬁrst time that such an event is held in Nlogonia.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The project, however, is still being worked on. ACM didn’t announce the list of host</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">cities yet, but, instead, it announced how the cities will be chosen. It’s worth mentioning</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">that Nlogonia was attacked by some kind of giant cannon in 2009, so the facilities in the cities</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">are damaged and can’t be fully considered (at least not now). Instead, a city will be chosen</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">according to how easy its name is pronounced.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Let’s deﬁne the pronunciation power (pp) of a city name S as the sum of the lengths of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">all its palindromic contiguous substrings with even positive length. For example, consider the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">name abbaxx. Its substrings with even positive length are {ab, bb, ba, ax, xx, abba, bbax, baxx,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">abbaxx}. Of these, the palindromic ones are {bb, xx, abba} and thus pp(abbaxx) = |bb| +</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">|xx| + |abba| = 8. Repeated substrings should be considered as many times as they occur (so</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">pp(aaa) = |aa| + |aa| = 4, since aa occurs twice). Also, letter comparisons are case insensitive</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">(so pp(aBbAxX) = 8, too), since the pronunciation is independent of the letter case.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Nlogonia has N cities. Let K be a number given by ACM. The cities whose names have a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">pronunciation power equal or greater than the K th unique highest power of all N cities will be</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">chosen. Notice that it’s possible to choose more than K cities. For example, consider K = 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and N = 6 cities whose names have the powers 2, 4, 4, 8, 8 and 16. The ﬁrst 3 unique higher</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">powers are 16, 8 and 4, so all cities except the ﬁrst one will be chosen.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The 2009 cannon attack also damaged the roads between the cities. There’are only M</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">one-way roads available to use in Nlogonia (if a road connects city A to B, it can’t be used to</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">go from B to A). Also, due the damages made by the cannon, each road has a traﬃc ﬂow limit.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Nlogonia’s capital is the only city with an airport, so all the foreign people will come to</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Nlogonia via the capital and go to the host cities using the road network cited above. Your</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">task is to help the Nlogonian people know the list of cities that will be chosen, and, for each</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">one, know what is the maximum traﬃc ﬂow possible from the capital to the city, so they</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">know if the roads will handle the traﬃc well during the event. During the World Cup, each</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">match will be played in a diﬀerent date and city, so consider the chosen cities independently</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">(in other words, calculate the ﬂow between the capital and the ﬁrst chosen city as if it was</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 5px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">the only chosen one; then do the same with the second chosen one, and so on).</div>
<p>&nbsp;</p>
<p>Nlogonian people is very excited about the event that will occur in the next year: the</p>
<p>Cheese-rolling World Cup Nlogonia 2013! The event is organized by the Modern Cheeserolling Association (MCA or ACM, as spelled in Nlogonish) every four years, and this will be</p>
<p>the ﬁrst time that such an event is held in Nlogonia.</p>
<p>The project, however, is still being worked on. ACM didn’t announce the list of host</p>
<p>cities yet, but, instead, it announced how the cities will be chosen. It’s worth mentioning</p>
<p>that Nlogonia was attacked by some kind of giant cannon in 2009, so the facilities in the cities</p>
<p>are damaged and can’t be fully considered (at least not now). Instead, a city will be chosen</p>
<p>according to how easy its name is pronounced.</p>
<p>Let’s deﬁne the pronunciation power (pp) of a city name S as the sum of the lengths of</p>
<p>all its palindromic contiguous substrings with even positive length. For example, consider the</p>
<p>name abbaxx. Its substrings with even positive length are {ab, bb, ba, ax, xx, abba, bbax, baxx,</p>
<p>abbaxx}. Of these, the palindromic ones are {bb, xx, abba} and thus pp(abbaxx) = |bb| +</p>
<p>|xx| + |abba| = 8. Repeated substrings should be considered as many times as they occur (so</p>
<p>pp(aaa) = |aa| + |aa| = 4, since aa occurs twice). Also, letter comparisons are case insensitive</p>
<p>(so pp(aBbAxX) = 8, too), since the pronunciation is independent of the letter case.</p>
<p>Nlogonia has N cities. Let K be a number given by ACM. The cities whose names have a</p>
<p>pronunciation power equal or greater than the K th unique highest power of all N cities will be</p>
<p>chosen. Notice that it’s possible to choose more than K cities. For example, consider K = 3</p>
<p>and N = 6 cities whose names have the powers 2, 4, 4, 8, 8 and 16. The ﬁrst 3 unique higher</p>
<p>powers are 16, 8 and 4, so all cities except the ﬁrst one will be chosen.</p>
<p>The 2009 cannon attack also damaged the roads between the cities. There’are only M</p>
<p>one-way roads available to use in Nlogonia (if a road connects city A to B, it can’t be used to</p>
<p>go from B to A). Also, due the damages made by the cannon, each road has a traﬃc ﬂow limit.</p>
<p>Nlogonia’s capital is the only city with an airport, so all the foreign people will come to</p>
<p>Nlogonia via the capital and go to the host cities using the road network cited above. Your</p>
<p>task is to help the Nlogonian people know the list of cities that will be chosen, and, for each</p>
<p>one, know what is the maximum traﬃc ﬂow possible from the capital to the city, so they</p>
<p>know if the roads will handle the traﬃc well during the event. During the World Cup, each</p>
<p>match will be played in a diﬀerent date and city, so consider the chosen cities independently</p>
<p>(in other words, calculate the ﬂow between the capital and the ﬁrst chosen city as if it was</p>
<p>the only chosen one; then do the same with the second chosen one, and so on).</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The input will consist of one or more test cases. Each test case starts with a line containing</p>
<p>three integers N (1 ≤ N ≤ 200), M (1 ≤ M ≤ N (N − 1)) and K(1 ≤ K ≤ 10). The cities are</p>
<p>numbered from 0 to N − 1, and the capital is the city number 0. Each of the N next lines</p>
<p>contains the names of the cities, in increasing order of their numbers. Each name will contain</p>
<p>only upper and lower case English letters, and its length will not exceed 30000. Each of the</p>
<p>M next lines will describe the road network of the country. Each line will be in the form A</p>
<p>B C (0 ≤ A, B &lt; N, A = B, 1 ≤ C ≤ 109 ) and indicates a road connecting city A to city</p>
<p>B with traﬃc ﬂow limit C. There won’t be more than one road connecting a pair of cities</p>
<p>in the same direction, and it will always be possible to go from the capital to any other city.</p>
<p>The last test case will be followed by a line containg three zeros.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each test case, print one line with k - the number of chosen cities. Then, print k</p>
<p>lines in the format n (pp) f , where n is a city name, pp is its pronunciation power and f is</p>
<p>the maximum ﬂow from the capital to the city. Print the cities in increasing order of their</p>
<p>numbers. Also, if the capital is a chosen city, use f = 0. You may assume that k ≤ 2K for</p>
<p>each test case.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 4 2
Curitiba
LalLal
Idappadi
0 1 2
2 1 1
0 2 3
1 2 6
4 5 3
heeymacarena
haay
abbaxx
ddxdd
0 3 20
0 2 10
2 3 5
3 1 10
2 1 20
0 0 0


<strong>Output:</strong>
2
LalLal (12) 3
Idappadi (20) 5
4
heeymacarena (2) 0
haay (2) 20
abbaxx (8) 10
ddxdd (4) 25
</pre>