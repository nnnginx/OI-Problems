<p>Summer's coming up in a few months, so you decide to hit the gym to put on some muscle. When you arrive, you're confronted with dozens of machines, free weights, barbells, stationary bikes and more. All of this is quite confusing to a newcomer, so you just stand there confused, checking your cellphone a few times, and leave.</p>
<p>After this less-than-stellar experience, you decide to do some research online. You learn that people train in things called "programs", which are instructions to determine how much weight to lift on a particular day. These are always of the form "Lift twice what you lifted three days ago, plus three times what you lifted 7 days ago", or similar. In general, such a "program" tells you that the weight you need to lift today is some combination of the weights you've lifted previously. The program also gives you some initial weights, for when the formula doesn't make sense.</p>
<p>Being very clever, however, you decide that the advice you find during your research is for suckers. You won't even bother with known programs like Starting Strength, StrongLifts 5x5, or even CrossFit. What you'll do is much cleverer: You'll go to the gym, find the most jacked bro in there, and imitate his program. To figure out his program, you'll record what he lifts each day he goes to the gym, for a few days.</p>
<p>Since you are lazy, of all the possible programs he could be following which would match your observations, you want only the shortest one (the one that mentions as few days back as possible). Can you find it?</p>
<h3>Input</h3>
<p>The input consists of multiple test cases, and starts with a positive integer T. T test cases follow.</p>
<p>Each test case starts with a number K, the number of days you've watched the bro lift weights for. After that come K nonnegative integers W_i, denoting the weight he lifted each day, from oldest lifts to most recent ones. You are assured that the bro is indeed following a program.</p>
<h3>Output</h3>
<p>For each test case, output a single line, consisting of N space separated non-negative integers D_i, if the program says each day you should lift the sum of (D_i times the weight you lifted i days ago), for 1 ¡Ü i ¡Ü N. N is the length of the shortest solution you found and should not be printed</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
10 48 64 96 128 192 256 384 512 768 1024
8 3 3 2 25 136 782 4479 25659 
8 3 3 24 87 381 1578 6639 27807
14 3 3 1 2 4 8 16 32 64 128 256 512 1024 2048 
8 16909 42737 110373 281321 722813 1848097 4739349 12131737</pre>
<pre><strong>Output:</strong>
0 2
5 4 1
3 5
2 0 0
1 4</pre>
<h3>Constraints</h3>
<div style="text-align: left;">1 ¡Ü T ¡Ü 5 * 10^3</div>
<div style="text-align: left;">1 ¡Ü K ¡Ü 44</div>
<div style="text-align: left;">K = 0 (mod 2)</div>
<div style="text-align: left;">0 ¡Ü W_i &lt; 2^63</div>
<div style="text-align: left;">In every program, K ¡Ý 2N.</div>
<div style="text-align: left;">Warning: You may need to use very big integers.</div>