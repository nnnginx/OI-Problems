<!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->
<p>You probably don't know toys walk, play and talk when we are not around. And there are toys who can perform intergalactic missions! But lets forget about alien planets now, the toy-land on earth is in danger, ¡°Zurg¡± the evil emperor from outer world is planning to capture it. But as always when toyland is in trouble the great space ranger ¡°Buzz Lightyear¡± of star command comes for the rescue!</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img title="Buzz" src="file://krgr8KTy.png" alt="Buzz" width="275" height="206"></p>
<p style="margin-bottom: 0in">Toyland consists of several cities and bidirectional roads. The Toyland chief wants to take following steps to save Toyland:</p>
<ol>
<li>First divide the cities of Toyland 	into multiple regions. <strong>Two cities  MUST be included in same region if 	there is at least one cyclic route  connecting both cities.</strong> <strong>One 	city can be included in multiple regions. </strong><span style="font-weight: normal;"> Size of each region should be maximal, that means extra city can't 	be added in a region.</span></li>
<li>There are 	limited number of ¡°Buzz¡± toys available. After creating the 	  regions, one ¡°Buzz¡± toy will be sent to each of them to save 	that   region from Zurg!</li>
</ol>
<p style="margin-bottom: 0in"><span style="font-weight: normal">Toys need energy. Each city can supply energy to infinite number of toys but the amount of energy a city provides daily to a single toy is limited otherwise toys may waste energy. </span><strong> A toy is assigned to a single region but it can get energy from any city with in its region.</strong></p>
<p style="margin-bottom: 0in; font-weight: normal">For a single toy, the total daily energy supply is sum of the energy supply of all the cities within its region.</p>
<p style="margin-bottom: 0in; font-weight: normal">Each ¡°Buzz¡± may need different amount of energy to work. If a region provides too less energy than additional energy need to be provided anyhow and it is considered as a lose. But if the region provides more energy than required,  ¡°Buzz¡± wastes it by playing with laser and flying all around.  So:</p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-size: x-small;"><strong>Daily Lose in region X = </strong></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-size: x-small;"><strong>| Daily Energy required by ¡°Buzz¡± assigned in that region - Daily  Energy supplied by region X |</strong></span></p>
<p style="margin-bottom: 0in" align="LEFT"><span style="font-weight: normal">Exactly one ¡°Buzz¡± must be assigned in each region, if there are more toy than needed, they'll keep them for emergency.</span><strong> </strong><span style="font-weight: normal">The chief wants to </span><strong>minimize the maximum wastage among all the regions </strong><span style="font-weight: normal">and he needs your help desperately. </span></p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">Help the toyland to survive, expand your mind To Infinity and Beyond and find the answer.</p>
<p style="margin-bottom: 0in" align="LEFT"><strong>Input Specification:</strong></p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">Input consists of several files. First line of each file will consist the number of test cases(T&lt;=101). For each case, first line will consists number of cities (1&lt;=N&lt;=251) , roads(E&gt;=0) and number of Buzz toys available(1&lt;=B&lt;=251). In next line there are N integers less than 1000, i-th integer denotes energy supply in city i. In next line there are B integers less than 1000, j th integer denotes energy required by Buzz j. Next there are E lines each consisting two integer u and v denoting there is a bidirectional road between u and v(u!=v).  There are at most one roads between two cities. All inputs are non-negative.</p>
<p style="margin-bottom: 0in" align="LEFT"><strong>Output Specification:</strong></p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">First print number of regions. Than if number of regions is more than number of buzz available, output ¡°No¡±.  Otherwise print the maximum wastage amount among all the regions. Dont print any extra spaces or newlines. Print case number for every case, see sample output for details.</p>
<p style="margin-bottom: 0in" align="LEFT"><strong>Large input File, use faster I/O.</strong></p>
<p style="margin-bottom: 0in" align="LEFT"><strong>Sample input:</strong></p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">2</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">6 7 3</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">5 4 8 1 2 6</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">10 14 9</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">1 2</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">2 3</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">3 1</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">3 4</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">4 5</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">3 5</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">5 6</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">4 3 1</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">5 4 8 1</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">10</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">1 2</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">2 3</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">3 1</p>
<p style="margin-bottom: 0in" align="LEFT"><strong>Sample Output:</strong></p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">Buzz Mission 1: 3 3</p>
<p style="margin-bottom: 0in; font-weight: normal" align="LEFT">Buzz Mission 2: 2 No</p>
<p style="margin-bottom: 0in" align="LEFT"><img title="Case 1 Explanation" src="file://YmIQGCSA.png" alt="Case 1 Explanation" width="368" height="297"></p>