<p>N (1 ¡Ü N ¡Ü 50,000) cows conveniently numbered 1, ..., N are driving in separate cars along a highway in Cowtopia. Cow i can drive in any of M different high lanes (1 ¡Ü M ¡Ü N) and can travel at a maximum speed of S<sub>i</sub> (1 ¡Ü S<sub>i</sub> ¡Ü 1,000,000) km/hour.</p>

<p>After their other bad driving experience, the cows hate collisions and take extraordinary measures to avoid them. On this highway, cow i reduces its speed by D (0 ¡Ü D ¡Ü 5,000) km/hour for each cow in front of it on the highway (though never below 0 km/hour). Thus, if there are K cows in front of cow i, the cow will travel at a speed of max(S<sub>i</sub> - D*K, 0). While a cow might actually travel faster than a cow directly in front of it, the cows are spaced far enough apart so crashes will not occur once cows slow down as described.</p>

<p>Cowtopia has a minimum speed law which requires everyone on the highway to travel at a a minimum speed of L (1 ¡Ü L ¡Ü 1,000,000) km/hour, so sometimes some of the cows will be unable to take the highway if they follow the rules above. Write a program that will find the maximum number of cows that can drive on the highway while obeying the minimum speed limit law.</p>


<h3>Input</h3>
<p>The first line contains the four integers N, M, D, and L. For the next N lines, line i+1 contains the integer S<sub>i</sub>.</p>

<h3>Output</h3>
<p>Print a single integer denoting the maximum number of cows that can take the highway.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3 1 1 5
5
7
5

<b>Output:</b>
2
</pre>

<p>We can obtain two cows by putting either cow with speed 5 first and the cow with speed 7 second.</p>