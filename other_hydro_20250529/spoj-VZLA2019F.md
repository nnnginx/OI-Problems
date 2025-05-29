<p><br>I live for a world full of chaos, mayhem is my dream. Sadly, friendship bonds keep the world together. \textbf{This has to end}. Initially, there are <strong>N</strong> people living in the world, and I know the strength of each one and the friendship bonds between them. A group of connected people will sum up their strengths if attacked (the power of friendship... <em>disgusting</em>, right?), so I'm interested in the strength of full groups of connected people, specially in the maximum strength of a group.<br><br>I have already set a plan of action, the order in which I will destroy friendships! But, turns out, that when one destroys friendships, people may react and increase or decrease their strength. I need your help to find out how successful my plan is.<br><br>I'll give you the initial information (strengths and bonds) and a list of <strong>Q</strong> events, each event will be either a destruction event, or a strength change event.<br><br>I need to know the maximum strength of a group after each event.</p>
<h3>Input</h3>
<p>The first line of input consists of two integers <strong>N</strong> and <strong>M</strong>, the number of people and the initial number of bonds respectively.<br><br>Next line will contain <strong>N</strong> integers s<sub>1</sub>, s<sub>2</sub>,... s<sub>N</sub> separated with exactly one white space, being s<sub>i</sub> the initial strength of the i-th person.<br><br>Next <strong>M</strong> lines will contain two integers a<sub>i</sub> and b<sub>i</sub>, representing a friendship bond between those two people.<br><br>The next line will contain a single integer <strong>Q</strong>, the number of events.<br><br>The following Q lines will be either:<br>• 1 k: Indicating the destruction of bond number k (in the input order)<br>• 2 p x: Indicates that the person p changed her strength to x</p>
<h3>Output</h3>
<p>Print Q lines, the maximum strength of a group after each event.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 6<br>3 3 3 3 3<br>1 2<br>1 3<br>2 3<br>2 5<br>3 4<br>4 5<br>5<br>2 1 2<br>1 5<br>1 4<br>2 4 8<br>2 3 7

<strong>Output:</strong>
14<br>14<br>8<br>11<br>12 </pre>
<h3>Constraints</h3>
<p>• 1 ≤ N, M, Q ≤ 10<sup>5</sup></p>
<p>• 1 ≤ s<sub>i</sub> , x<sup><sub>i</sub></sup> ≤ 10<sup>5</sup></p>
<p>• 1 ≤ a<sub>i</sub> , b<sub>i</sub> ≤ N</p>
<p>• 1 ≤ k<sub>i</sub> ≤ M</p>
<p>• 1 ≤ p<sub>i</sub> ≤ N</p>
<p>• every bond will be deleted at most once.</p>
<p>• between two people there is at most one bond.</p>