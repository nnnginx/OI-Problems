<p>&nbsp;</p>
<p>The King of Thuvax decided to conquer the neighbouring country of Silicon Valley. In order to conquer &nbsp;a country, he has to successfully invade every city in the country. But he always doesn't get into action unless he plans it properly. He knows that severing a city's communications with all other cities before invading it is the only way to conquer it. He has the information regarding how the cities communicate with each other through his spy. The spy has lived in Silicon Valley right from the time when it was a single city, much before its development into a country. He gives information about how every new city established communication links with other cities. The spy's information is represented as below.</p>
<p>&nbsp;</p>
<p>Every city can establish its communications with the help of only one other city. It can do it in one of the three ways.</p>
<p>Type 1-It can establish a single communication link with another city 'c'.</p>
<p>Type 2-It can establish communication links with all cities that communicate with another city 'c', but it can't have a communication link with 'c'.</p>
<p>Type 3-It can establish communication links with all cities that communicate with another city 'c' and with 'c' also.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>All communication links are two-way. Having this information, he finds out that it is not possible for him to invade Silicon Valley in a fair way. So he hires a terrorist gang to bomb some cities and destroy them so that he can invade the country successfully. But the terrorists demanded a huge amount of money for bombing a city. Help the King to find out the minimum number of cities that should be bombed so that he can conquer the country of Silicon Valley successfully.</p>
<p>&nbsp;</p>
<p>Input</p>
<p>&nbsp;</p>
<p>The first line consists of number of test cases t(1&lt;=t&lt;=10)</p>
<p>The first line of each test case consists of the number of cities n(1&lt;=n&lt;=10^4) in Silicon Valley.</p>
<p>Each of the next n-1 lines consists of two integers x and c.</p>
<p>The ith(1&lt;=i&lt;=n-1) line represents that city i+1 establishes a type 'x' communication link with the help of the city 'c'(1&lt;=c&lt;=i).(The country initially contains city 1 alone.)</p>
<p>&nbsp;</p>
<p>Output</p>
<p>&nbsp;</p>
<p>Output one line for each test case containing the minimum number of cities that should be bombed so that the King can conquer the country.</p>
<p>&nbsp;</p>