The Agents need to unite. They are on a road and each of them possess a special device which can both send and receive signals, in both directions upto a maximal distance of D units. Apart from this small limitation, the devices work very efficiently so that the time
taken for interdevice communication is practically zero. Now that the agents are at different points on the road, for them to be able to communicate with each other at will, every agent should be connected to every other agent through one or more intermediate devices. For
example: agent A may communicate to agent C via agent B¡¯s device, when A and C are not close enough. This happens when <strong>dist</strong>(A,C)&gt;D, but <strong>dist</strong>(A,B)&lt;=D and <strong>dist</strong>(B,C)&lt;=D.<p></p>

<p>Getting the line ready, is the process of agents moving from their current positions in order to get the network fully connected. That is, from every agent to every other agent, there is a communication path. </p>

<p>The agent¡¯s final positions (in two cases that are going to follow) are decided by a programmer, who watches the scene from above and instructs each agent of the time to move and the final position to move to. Each agent moves a unit distance in unit time.</p>

<p>We need to find the minimal time taken for the programmer to ¡°get the line ready¡± if he moves the agents:<br>

1. Independently: In other words, every agent moves to their final
position without waiting for any other agent; all agents are told of
their final positions at time zero.<br>
2. Sequentially: In this the agents form a definite sequence of movement. No two agents are moving at the same time.</p>
<h3>Input</h3>
<p>T ¨C number of test cases. For each test case :<br>
  N D ¨C where N is the number of agents, D is the maximal communication distance<br>
  The i-th line, of the N-lines that follow gives the position of the i-th agent on the road currently.</p>
<h3>Output</h3>
<p>For each test case, output two integers;<br>
1st ¨C minimal time taken to unite if they move independently<br>
2nd - minimal time taken to unite if they move sequentially</p>
<p><strong>Constraints:</strong><br>
  T&lt;=20<br>
  1&lt;=N,D&lt;=100 ; <br>

  Each agent's initial position is between 0 and 1000.</p>

<h3>Example</h3>
<pre><strong>Sample Input:</strong>
2
4 3
10 20 30 35
5 3
1 2 3 4 30

<strong>Sample Output:</strong>
8 23
12 23</pre>