<p>Ciempierre is a funny <em>n-pede</em>, and arthropod with exactly <strong>N</strong> <strong></strong>legs. He likes clothing, and today he bought <strong>N</strong> different shoes and <strong>N</strong> different socks. To get dressed, he has to put exactly one sock and one shoe on every leg. <br><br>He is a bit eccentric, and he wants to get dressed every morning in a <em>different way</em>. He defines a way of getting dressed as the order he puts his clothes on. In one step, he can choose one leg and one sock <strong>or</strong> one shoe. Two ways of getting dressed are different if there is at least one step where he chooses a different leg or, in case of using the same leg, a different sock or shoe.<br><br>For example, if Ciempierre has two legs he will buy two different socks and two different shoes. One way of getting dressed is:</p>
<p>1. Put sock 1 on leg 1<br>2. Put sock 2 on leg 2<br>3. Put shoe 1 on leg 1<br>4. Put shoe 2 on leg 2<br><br>Notice that two ways are not neccesarily equal if they make Ciempierre look the same. For example, if we swap the first and second steps on the example explained above, it would have been a different way of getting dressed, but his look would had been the same.<br><br>Not all the ways of getting dressed are valid, though. Ciempierre can't put a shoe on a leg <strong>before</strong> putting a sock on that leg first.<br><br>Given the number of legs Ciempierre has, can you calculate the number of different ways he can get dressed?</p>
<h3>Input</h3>
<p>The first and only line of the input will have an integer <strong>N</strong>, being the number of legs Ciempierre has, and for instance the number of different socks and different shoes he bought.</p>
<h3>Output</h3>
<p>Print the number of different ways he can get dressed. As this number can be really big, you must print it modulo 10^9 + 7</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2

<strong>Output:</strong>
24<br><br><strong>Input:<br></strong>3<br><br><strong>Output:<br></strong>3240<br><br><strong>Input:<br></strong>1<br><br><strong>Output:<br></strong>1<br><br><strong>Input:<br></strong>10<br><br><strong>Output:</strong><br>540458589 </pre>
<h3>Constraints</h3>
<p>1 ¡Ü N ¡Ü 10^5</p>