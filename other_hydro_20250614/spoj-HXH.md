<p><span style="font-size: small;">Gon and Killua are two very talented hunters, and they are also very skilled fighters, however it is well known that Killua is faster and smarter than Gon, and Gon is stronger and is way more decided than Killua. That makes them almost the perfect team (they just need more time to become the most skilled hunters that ever lived) and they are so good as a team that they decided to fight and defeat many enemies (as much as they can) so they made a plan, as the enemies are in a N x N grid Gon decided to start at position 0,0 of this grid and Killua at position n-1,n-1. To maximize the number of defeated enemies Gon moves only to the Right and Down, and Killua to the Left and Up, they count how many enemies they defeated and stop when both of them are in the same cell and they give each other a high five. So if they complete the ride without doing this they will be mad, so that will not be a solution.</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">However Killua wants this to be perfect, so he is tracing a new plan, but he does not know the best ride, as you are an amazing programmer he asked you for your help and you need to give him the maximum amount of enemies they can defeat together and then give each other a high five, only with this information the super brain of Killua will figure out the rest.</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">Remember, the ride will not finish if they do not give each other that high five.</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">The grid has this properties:</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">¡®#¡¯ is an obstacle that neither Gon nor Killua can pass through</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">¡®.¡¯ Is a walkable area</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">¡®*¡¯ is an enemy</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">Also they move at the same time, if any of them cannot move, it will not be a valid move. They never stand still.</span></p>
<h3>Input</h3>
<p><span style="font-size: small;">The input consist on several test cases represented by T each of them start with an 2&lt;=N&lt;=500 the size of the grid and the grid itself.</span></p>
<p>&nbsp;</p>
<p><span style="font-size: small;"><strong>Output</strong></span></p>
<p><span style="font-size: small;">Just show the maximum number of enemies that both can defeat, and then give each other a high five. If this cannot be done print -1<br></span></p>
<p>&nbsp;</p>
<p><span style="font-size: small;"><strong>Input test:</strong></span></p>
<p><span style="font-size: small;">1</span></p>
<p><span style="font-size: small;">5</span></p>
<p><span style="font-size: small;">..*..</span></p>
<p><span style="font-size: small;">.*..*</span></p>
<p><span style="font-size: small;">#...*</span></p>
<p><span style="font-size: small;">..*..</span></p>
<p><span style="font-size: small;">.....<br></span></p>
<p><span style="font-size: small;"><strong>Output test:</strong></span></p>
<p><span style="font-size: small;">3</span></p>
<p>&nbsp;</p>
<p><span style="font-size: small;">They could defeat all 5 if they weren¡¯t going to give each other a high five, but as they do and they never stand still, they will defeat only 3 and then give a High five, Killua defeats 2 and Gon 1.</span></p>
<p>&nbsp;</p>