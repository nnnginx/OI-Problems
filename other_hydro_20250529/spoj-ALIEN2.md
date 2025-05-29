<p>The Alien who doesn¡¯t like to see humans has moved to an Urban City (Yes, a little ironic) and now she¡¯s facing a double-train system, but still, the alien hates humans, so she wants to see the minimum quantity of people possible in her way to the university at the two trains.</p>
<p>The Alien has some sort of anthropophobia, this means she has a phobia to the people or the society, knowing this, she tells you that can only see K persons in the train, if she sees more than that, she will have a panic attack.</p>
<p>With her special powers, the alien knows how much people is on every station of the train A and the train B, she asked you to make a program that, given the number of people in the stations of the train A and B and the maximum number of people she wants to see, you give her the number of stations she will have to cross and the minimum persons found in those stations. Knowing that:</p>
<ul>
<li>The Alien starts from train A or B (she can choose where to start) but from the station 1.</li>
<li>She can switch from train A or B or viceversa, if she does this, she will see Ai+Bi people, being ¡°i¡± the station she¡¯s at that moment.</li>
<li>If she sees strictly more persons than the specified, she will automatically exit the train.</li>
</ul>
<p><strong>INPUT:</strong></p>
<p>The input will contain two integers N (1&lt;=N&lt;=10,000) and K (1&lt;=65,000) being the number of stations and the maximum number of people that the alien wants to see, then, 2 lines will follow, each containing N integers separated by a single space denoting the number of people found in the j-th station of the i-th train. (1&lt;=Ni&lt;=100)</p>
<p><strong>OUTPUT:</strong></p>
<p>Two single numbers denoting the number of stations passed and the people seen.</p>
<p>&nbsp;</p>
<p><strong>SAMPLE DATA:</strong></p>
<p><strong>INPUT:</strong></p>
<p>3 10</p>
<p>9 2 4</p>
<p>1 2 9</p>
<p><strong>OUTPUT:</strong></p>
<p>3 9</p>
<p><strong>INPUT2:</strong></p>
<p>5 10</p>
<p>1 7 1 1 1</p>
<p>2 2 2 2 2</p>
<p><strong>OUTPUT2:</strong></p>
<p>5 9</p>
<p>&nbsp;</p>
<p>Explanation I/O 1: The alien starts at the train B station 1, she sees 1 people, she continues to the station 2 and then decides to change the train, the alien have seen 4 more people, and then she continues at the train A up to the station 3. At this point the Alien will see (1+4+4) people (9) and has passed 3 stations.</p>