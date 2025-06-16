<p>Ada the Ladybug just got an inovative idea (which might be a rival of captcha): She made following function - <strong>F(a)=least significant 1-bit of a</strong> (indexed from 1). She also made following recursive function <strong>T(N)=F(N*(N-1))<sup>3</sup>+T(N-2)</strong>, where <strong>T(0)=0,T(1)=0</strong>.</p>
<p>Her idea is following- Instead of asking for captcha, she uses an opposite method: She gives you even <strong>N</strong> and you have to answer <strong>T(N)</strong> - if your answer is correct, then you are definetly robot and you won't be let in.</p>
<p>As her good friend she asked you to program a checker for her.</p>
<h3>Input</h3>
<p>The input begins with an integer <strong>1 ¡Ü Q ¡Ü 10<sup>6</sup> </strong>, number of queries.</p>
<p>The next <strong>Q</strong> lines contains an even integer: <strong>2 ¡Ü N ¡Ü 2*10<sup>8</sup></strong></p>
<h3>Output</h3>
<p>For each query, print <strong>T(N)</strong></p>
<h3>Example Input</h3>
<pre>5
8
4
2
20
1000
</pre>
<h3>Example Output</h3>
<pre>107
35
8
310
23988
</pre>
<h3>Little explanation</h3>
<pre>F(2)=2
F(12)=3
F(30)=2
F(56)=4
F(90)=2
F(132)=3
F(182)=2
F(240)=5
F(306)=2
F(380)=3
</pre>