<p><em>Profiling: In software engineering, profiling ("program profiling", "software profiling") is a form of dynamic program analysis that measures, for example, the space (memory) or time complexity of a program, the usage of particular instructions, or the frequency and duration of function calls. Most commonly, profiling information serves to aid program optimization.&nbsp; </em></p>
<p><em><span style="white-space: pre;"> </span>Wikipedia</em></p>
<p>&nbsp;</p>
<p>Arthur and Jacob are newly introduced to the programming world and they are trying hard for Newbies contest. Yesterday, they learned about recursive functions and Fibonacci sequence. They tried to implement the function themselves so they wrote the following code:</p>
<p>int fibonacci (int N)</p>
<p>{</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(N &lt; 2)</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return N;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return fibonacci(N - 1) + fibonacci(N - 2);</p>
<p>}</p>
<p>But this program works slowly when N is a large number. They traced the program and found the cause of this problem. Take a look at the following picture:</p>
<p><img title="Fibonacci Sequence Tree" src="./23991/file/hKaO86kD.png" alt="Fibonacci Sequence Tree" width="604" height="219"></p>
<p>If you want to calculate Fibonacci(6), Fibonacci(3) will be calculated multiple times!</p>
<p>They want to know how serious this problem can be, so they need a profiler to calculate such a thing for them.</p>
<p>Your task is to provide the profiler which receives two integers N, K and tells them if they call Fibonacci(N) how many times Fibonacci(K) will be calculated (according to their code).</p>
<h3>Input</h3>
<p>The first line of input indicates the number of test cases (There will be at most 100 test cases)</p>
<p>For each test case, there are two space-separated integers N, K &nbsp;in a single line. (0¡ÜN,K¡Ü10<sup>5</sup>)</p>
<h3>Output</h3>
<p>For each test case, print the number of times Fibonacci(K) will be calculated, if we call Fibonacci(N). Since the result can be very large, print the result modulo (Mod %) 1000000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
6 6
6 3
6 2
100000 3
5 10

<strong>Output:</strong>
1
3
5
855252772
0</pre>