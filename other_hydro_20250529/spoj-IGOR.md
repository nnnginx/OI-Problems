<p>Dr Samuel has been working in one of his grim (and useless) experiments in order to take control of the humanity.</p>
<p>Recently, he has been working in a hypnotic bomb, and he plans to launch it in the center of the city. Once it falls, all the inhabitants will be under his control, due to the properties of its principal element, the Samuelanium.</p>
<p>Amusingly, the Doctor himself created this element, and he does not know its behavior! He has commanded Igor, his faithful sidekick (and slave) to describe it.</p>
<p>Samuelanium��s behavior is pretty strange. According to Igor��s Notes:</p>
<p>-Its atoms are only composed by electrons and protons and it has a chain-like shape.</p>
<p>-On its sides there are two strange portals. They can suck the proton-electron chain in only one direction. Once a particle enters in a portal, it comes back from the other portal with its charge changed.</p>
<p>-If the first particle in the chain is a proton, the charge of the last particle changes.</p>
<p>For example, suppose we have the chain "+-+".</p>
<p>As you can see, the first particle is a proton, so the last particle must change its charge, becoming "+--". Then, the chain is sucked by the left portal. The proton comes out from the right portal, having changed it charge, becoming "---"(as an electron). This occurs in one second.</p>
<p>So, if the chain is represented as "+-+" at time 0, it will be represented as "---" at time 1.</p>
<p>Doctor Samuel wants to know the state of this chain, having passed some seconds from its initial state.</p>
<p>Unfortunately, Igor is exhausted. Can you help Igor and (ironically) help Doctor Samuel to control the humanity and conquer the whole world?</p>
<h3>Input</h3>
<p>Your program will be tested with t experiments.</p>
<p>Every experiment begins with two integers, n and k. n represents the length of the Samuelanium chain, and k represents the number of queries that Samuel demands.</p>
<p>Next, there will be a string of length n, composed only of '+' and '-'. '+' represents a proton, and '-' an electron. This chain represents its initial state (time 0).</p>
<p>You must assume that the portal that sucks the chain is on the left side.</p>
<p>Then, there will be k lines, with an integer ki, representing the time query you have been asked for.</p>
<h3>Output</h3>
<p>For each test case you must print one line containing "Experiment #i:", being i the ith case you are analyzing.</p>
<p>Then, k strings, representing the chain in a given moment.</p>
<p>Remember, protons are represented with '+' and electrons with '-', and there are no neutrons.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>1</p><p>3 4</p><p>+-+</p><p>0</p><p>1</p><p>2</p><p>4</p><strong>Output:</strong>
<p>Experiment #1:</p><p>+-+</p><p>---</p><p>--+</p><p>+++</p><p><strong>Constraints:</strong></p><p>1&lt;=t&lt;=15</p><p>1&lt;=n&lt;=14</p><p>10&lt;=k&lt;=1000</p><p>0&lt;=ki&lt;=10^9</p></pre>