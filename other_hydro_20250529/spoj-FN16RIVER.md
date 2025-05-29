<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The Chao Phraya River System is the main river system of     Thailand. Its six     longest rivers listed by decreasing length are:</p>
<ol class="enumerate">
<li>
<p>Tha Chin ($765$         km)</p>
</li>
<li>
<p>Nan ($740$ km)</p>
</li>
<li>
<p>Yom ($700$ km)</p>
</li>
<li>
<p>Ping ($658$ km)</p>
</li>
<li>
<p>Pa Sak ($513$         km)</p>
</li>
<li>
<p>Wang ($335$ km)</p>
</li>
</ol>
<p>A simplified model of this river system is shown in     figure below, where the smaller red numbers indicate the     lengths of various sections of each river. The point where two     or more rivers meet as they flow downstream is called a     <em>confluence</em>. Confluences are labeled with the larger     black numbers. In this model, each river either ends at a     confluence or flows into the sea, which is labeled with the     special confluence number      $0$. When two or more rivers meet at a     confluence (other than confluence      $0$), the resulting merged river takes     the name of one of those rivers. For example, the Ping and the     Wang meet at confluence      $1$ with the resulting merged river     retaining the name Ping. With this naming, the Ping has length     $658$ km while the Wang is     only $335$ km. If instead     the merged river had been named Wang, then the length of the     Wang would be $688$ km     while the length of the Ping would be only      $305$ km.</p>
<p><img style="width: 450px; height: 230px;" src="../../../content/john_jones:fn16river.png" alt=""></p>
<p>The raised awareness of this phenomenon causes bitter     rivalries among the towns along the rivers. For example, the     townspeople along the Wang protest that maybe with a proper     naming scheme, their river could actually be the longest, or     maybe the second longest (or at least not last!). To end all     the guessing, your task is to validate all such claims.</p>
<p>The <em>rank</em> of a river is its position in a list of     all rivers ordered by decreasing length, where the best rank is     $1$ for the longest river.     For each river, determine its best possible rank over all     naming schemes. At any confluence, the name of a new, larger     river in any naming scheme must be one of the names of the     smaller rivers which join at that confluence. If two or more     rivers have equal lengths in a naming scheme, all the tied     rivers are considered to have the best possible ranking. For     example, if one river is the longest and all other rivers are     equal, those rivers all have rank      $2$.</p>
<h3>Input</h3>
<p>The first line of input contains two integers      $n$ $(1     \le n \le 500\, 000)$, which is the number of river     sources in the system, and      $m$ $(0     \le m \le n - 1)$, which is the number of confluences     with positive labels. These confluences are numbered from     $1$ to      $m$.</p>
<p>The next $n$ lines     describe the rivers. Each of these lines consists of two integers     $c$      $(0 \leq c \leq m)$ and      $d$ $(1     \leq d \leq 10^9)$, where      $c$ is the identifier of the nearest     confluence downstream, and      $d$ is the distance from the source to     that confluence in kilometers.</p>
<p>The final $m$ lines     describe confluences $1$     to $m$ in a similar     fashion. The $k^\text     {th}$ of these lines describes the confluence with     identifier $k$ and     contains two integers: the identifier of the nearest confluence     downstream and the distance from confluence      $k$ to this confluence in     kilometers.</p>
<p>It is guaranteed that each confluence      $1$ through      $m$ appears as ¡°the nearest     downstream¡± at least twice, confluence      $0$ appears at least once, and all     sources are connected to confluence      $0$.</p>
<p><strong>Due to the input file size limit, all numbers given in the input file is written in base 64 integers. Base 64 integer uses 0-9 to denote number 0 - 9, A-Z to denote number 10 - 35, a-z to denote number 36 - 61, + to denote number 62 and / to denote number 63.</strong></p>
<h3>Output</h3>
<p>Display one river per line in the same order as in the     input. On that line, display the river's best     possible rank (in decimal notation).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 2
0 81
2 AZ
2 Ay
1 5F
1 4n
0 Bz
0 5X
0 11

<strong>Output:</strong>
5
2
1
3
4
1

<strong>Input:</strong>
6 3
1 GN
2 fQ
1 CW
3 B6
0 h/
3 CJ
2 1a
0 Qa
0 U

<strong>Output:</strong>
1
1
3
6
1
4
</pre>