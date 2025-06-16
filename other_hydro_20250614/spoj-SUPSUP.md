<p>It's battle time yet again, and now General Frey is worried about the supplies to his units. The capital city of the Empire has two exits, the North Gate and the South Gate, at which several key elements to the army will be stored. Several squads are going to be deployed, and seeing as each one of them has different needs, the General needs to decide on which exit he will deposit each supply type. Storing a supply element on both exits is costly and confusing, so the whole shipment for a resource must be located at a single exit.</p>
<p>The orders that specify which soldier should get which supply should not be disrespected, that is, two soldiers from the same squad cannot swap items if it's more convenient to do so. To solve this issue, the General has decided that a simple rule should be followed: No squad should ever have more than one soldier carrying an element from the opposite exit in which he is located. Given the list of squads and their needs, find out if it's possible to place the items on the exits such that the rule's followed.</p>
<h3>Input</h3>
<p>The input consists of several test cases. On the first line of each test case will be an integer N (1 <span>¡Ü N </span><span>¡Ü 100)</span>, the number of squads. Each of the following N lines begins with an integer t, describing how many needs that specific squad has. t integers and characters follow, each of which specify a supply type that squad needs. You may assume a supply type fits in a signed 32-bit integer. If the character is 'S', then the soldier that is going to fetch that item is at the South Gate, if it is 'N' the soldier is at the North Gate. Equal integers specify equal supply types, and no item appears twice on the same squad list. The number of different supply types in a single testcase is at most 100.</p>
<p>The last test case will be followed by a line containing a single zero.</p>
<h3>Output</h3>
<p>Print a single line for each test case. The line must contain the words "March onward" if it's possible to assign the deposits and follow the General's rules, "Coordination issue" otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>2 1S 2S<br>2 1N 2N<br>2<br>3 1S 2S 3S<br>3 1N 2N 3N<br>0

<strong>Output:</strong>
March onward<br>Coordination issue</pre>