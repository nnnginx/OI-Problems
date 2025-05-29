<p>You have been monitoring a terrorist cell that is planning a big attack somewhere close. The terrorists have been sending encoded coordinates to each other, and you suspect that the attack will happen at one of the locations described by these coordinates. You have intercepted the relevant communications for a series of locations you want to investigate. Every location consists of a separate x and y coordinate, each being a non-negative integer smaller than some prime number P. Both coordinates are encoded separately using the same process. A source has given you information on the process of decoding a single coordinate. The input of this process consists of five values: A, B, C, K and N. Central to the decoding process is a collection of three functions, defined in terms of each other and the input value K:</p>
<p><strong>F(n + 1) = G(n) + H(n)</strong></p>
<p><strong>G(n + 1) = K * F(n) + H(n - 1)</strong></p>
<p><strong>H(n + 1) = F(n) + K * G(n)</strong></p>
<p>The values A, B and C are used to initialize these functions as follows:</p>
<p><strong>F(1) = A, G(1) = B, H(1) = C</strong></p>
<p>The decoded coordinate is the value of <strong>F(N) mod P</strong>. As you might have noticed, there is some crucial information missing: you need the value of H(0) to calculate G(2). While you do not have this value, you do know that the x and y coordinate use the same value for H(0). Luckily, you have managed to already obtain the x coordinates for the locations. Your colleagues have suggested that this does not give you enough information to calculate the y coordinates, but you want to prove them wrong.</p>
<h3>Input</h3>
<p>On the first line one positive number: the number of test cases, at most 100. After that per test case:</p>
<p> # one line with the prime number P (2 ¡Ü P ¡Ü 19997).</p>
<p> # one line with five space-separated integers Ax, Bx, Cx, Kx and Nx (0 ¡Ü Ax,Bx,Cx,Kx &lt; P and 1 ¡Ü Nx ¡Ü 10^9): the parameters for the x coordinate.</p>
<p> # one line with five space-separated integers Ay, By, Cy, Ky and Ny (0 ¡Ü Ay,By,Cy,Ky &lt; P and 1 ¡Ü Ny ¡Ü 10^9): the parameters for the y coordinate.</p>
<p> # one line with one integer x (0 ¡Ü x &lt; P): the x coordinate.</p>
<h3>Output</h3>
<p>Per test case:</p>
<p> # one line with one integer: the calculated y coordinate. If your colleagues are right, and there is not exactly one valid y coordinate, print ¡°UNKNOWN¡± on a single line instead.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
11
2 3 5 7 4
4 6 8 9 7
5
7
1 6 2 5 1
3 4 2 5 3
1

<strong>Output:</strong>
7
UNKNOWN
</pre>
<pre><strong>Notice : Extra spaces in output will cause <span style="color: #ff0000;">Wrong Answer</span></strong></pre>