<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">"Weddings are basically funerals with cake Morty"</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Birdperson has invited Rick and Morty to attend his marriage party. Rick doesn't like to go to marriage parties but Morty wants to go, as Birdperson is a very close friend. Also, Birdperson is king of Bird-planet and wants to compensate for the travel expenses for Rick's family. Bird-planet is many light years away from the earth but that is not the problem as Rick has Space Cruiser with hyperspeed.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Space cruiser needs 1 unit of fuel to travel 1 light year but it has a limited capacity 'C' so they may need to refuel in-between. There are many planets between Birdplanet and Earth and the fuel pricing is different on each planet.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Let Earth is numbered as '1' and bird-planet as 'N+1' then they can fuel at n planets (including earth). Distance between any two consecutive planets is 'D' light-years.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Evil Rick wants to maximize the expense of fueling and Birdperson knows this so he put a condition that on arrival there should be zero fuel in the tank.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Your task is to maximize the expense and it is obvious that they can't fuel at bird-planet. Initially, there is zero fuel in the tank.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">INPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains T, the number of test cases. Then the test cases follow.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line of each test case contains N, C and D, Number of planets for fueling (including earth), Capacity of the fuel tank and distance between two consecutive planets</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Second-line contains A1 A2 A3¡­ AN, where Ai denotes the price of 1 unit of fuel on ith planet.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">OUTPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each test case print the maximum possible expense.</div>
<blockquote>
<p>"Weddings are basically funerals with cake Morty"</p>
<p>&nbsp;</p>
</blockquote>
<p>Birdperson has invited Rick and Morty to attend his marriage party. Rick doesn't like to go to marriage parties but Morty wants to go, as Birdperson is a very close friend. Also, Birdperson is king of Bird-planet and wants to compensate for the travel expenses for Rick's family. Bird-planet is many light years away from the earth but that is not the problem as Rick has Space Cruiser with hyperspeed.</p>
<p>&nbsp;</p>
<p>Space cruiser needs 1 unit of fuel to travel 1 light year but it has a limited capacity 'C' so they may need to refuel in-between. There are many planets between Birdplanet and Earth and the fuel pricing is different on each planet.</p>
<p>&nbsp;</p>
<p>Let Earth is numbered as '1' and bird-planet as 'N+1' then they can fuel at n planets (including earth). Distance between any two consecutive planets is 'D' light-years.</p>
<p>&nbsp;</p>
<p>Evil Rick wants to maximize the expense of fueling and Birdperson knows this so he put a condition that on arrival there should be zero fuel in the tank.</p>
<p>&nbsp;</p>
<p>Your task is to maximize the expense and it is obvious that they can't fuel at bird-planet. Initially, there is zero fuel in the tank.</p>
<p>&nbsp;</p>
<h3>Input:</h3>
<p>The first line contains T, the number of test cases. Then the test cases follow.</p>
<p>&nbsp;</p>
<p>The first line of each test case contains N, C and D, Number of planets for fueling (including earth), Capacity of the fuel tank and distance between two consecutive planets</p>
<p>&nbsp;</p>
<p>Second-line contains A1 A2 A3¡­ AN, where Ai denotes the price of 1 unit of fuel on ith planet.</p>
<p>&nbsp;</p>
<h3>Output:</h3>
<p>For each test case print the maximum possible expense.</p>
<p>&nbsp;</p>
<h3>Constraints:</h3>
<p>1¡ÜT¡Ü10</p>
<p>1¡ÜN¡Ü10<sup>5</sup></p>
<p>1¡ÜD¡Ü10<sup>5</sup></p>
<p>D¡ÜC¡Ü10<sup>5</sup></p>
<p>1¡ÜAi¡Ü10<sup>9</sup></p>
<h3>Example:</h3>
<p>Input:</p>
<p>1</p>
<p>3 5 3</p>
<p>1 5 2</p>
<p>Output:</p>
<p>30</p>
<p>&nbsp;</p>
<p>Explanation:</p>
<p>-As N=3 so birdplanet will be 4th planet and hence they will need to travel 3*3=9 light year,</p>
<p>&nbsp;</p>
<p>-first they will buy 3 unit fuel from 1st planet to go to 2nd planet, expense: 3*1=3</p>
<p>&nbsp;</p>
<p>-They will buy 5 unit of fuel (up to full capacity) at 2nd planet, expense: 5*5=25</p>
<p>&nbsp;</p>
<p>-There will be 2 unit of fuel remaining on reaching 3rd planet so the need to buy only 1 more unit of fuel to reach Birdplanet, expense: 1*2=2</p>
<p>&nbsp;</p>
<p>-Total expense 3+25+2=30</p>
<p>&nbsp;</p>